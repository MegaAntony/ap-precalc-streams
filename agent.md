# Agent Operations Manual: Cloud Document & Stream Downloader
**Target Scope**: Cobb County High School Grade 9 (Antony)  
**Location**: `/Volumes/Backup/Antony/HighSchool/Grade9`  
**Purpose**: Playbook for future AI agents to authenticate, extract, batch-download, and publish protected school materials (PDFs, Videos, Answer Keys) without manual browser intervention.

---

## 1. System Architecture & Auth Mechanics

School resources (CTLS, Cobb Virtual Academy, MyVRSpot) protect learning resources across two layers:

| Resource Type | Hosting Platform | Protection Mechanism | Expiration Behavior |
| :--- | :--- | :--- | :--- |
| **Worksheets & Answer Keys** | CTLS / Cobb County Portal | AWS Application Load Balancer (`AWSALBTG`, `AWSALBTGCORS`) + Session Cookies | Bound to user login session; cookies expire after inactivity. |
| **Teacher Recorded Lessons** | MyVRSpot via AWS CloudFront CDN | AWS CloudFront Signed URLs (`Expires`, `Signature`, `Key-Pair-Id`) | Query tokens expire quickly (hours/days); hardcoded links return `403 Forbidden`. |
| **Supplementary Lessons** | YouTube (e.g. Mario's Math) | Public video IDs with iframe embedding | Permanent; no auth required. |

---

## 2. Playbook A: Downloading Protected PDFs & Worksheets

When new worksheets, test reviews, or answer keys are assigned on CTLS:

### Step 1: Capture Session Cookies
Ask the user for or grab a single `curl` command from DevTools (Network tab) for any protected PDF on CTLS. The header will look like:
```http
Cookie: AWSALBTG=...; AWSALBTGCORS=...; PHPSESSID=...; _csrf=...
```

### Step 2: Batch Download via Session Reuse
Use the captured cookie in a Python script or loop to download all required documents directly into the corresponding course folder.

```python
import requests

cookies = {
    'AWSALBTG': '<PASTE_COOKIE_HERE>',
    'AWSALBTGCORS': '<PASTE_COOKIE_HERE>'
}
headers = {
    'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36'
}

docs = {
    "Worksheet_Name.pdf": "https://school.portal.url/path/to/document.pdf",
    "Worksheet_Answers.pdf": "https://school.portal.url/path/to/answers.pdf"
}

for filename, url in docs.items():
    r = requests.get(url, cookies=cookies, headers=headers, stream=True)
    if r.status_code == 200:
        with open(filename, 'wb') as f:
            for chunk in r.iter_content(chunk_size=8192):
                f.write(chunk)
        print(f"Downloaded: {filename}")
    else:
        print(f"Failed {filename}: HTTP {r.status_code}")
```

### Step 3: Verify Integrity
Always verify downloaded files are actual PDFs and not HTML login redirects:
```bash
file "Worksheet_Name.pdf"
# Must output: PDF document, version ...
```

---

## 3. Playbook B: Downloading Protected CloudFront Videos (MyVRSpot)

Direct links to CloudFront MP4s (`d1drabmetuo3qr.cloudfront.net/....mp4?Expires=...`) expire and **must never be hardcoded**. Instead, use the dynamic embed endpoint to generate fresh signed download streams on demand.

### Step 1: Identify the MyVRSpot Media ID
The school provides links in one of two forms:
- Full URL: `https://live.myvrspot.com/iframe?v=MjgxNGFhYmQzODAwNGQxZGU4YmE1MWUxZTIyZDc4MWM`
- Media Key / Hash: `MjgxNGFhYmQzODAwNGQxZGU4YmE1MWUxZTIyZDc4MWM`

### Step 2: Extract Live Signed Stream URL
MyVRSpot's `/iframe?v=<ID>` endpoint dynamically injects fresh CloudFront signatures into the HTML `<source>` tags. Fetch and grep it:

```bash
# One-liner to extract the current valid high-res MP4 URL:
curl -s "https://live.myvrspot.com/iframe?v=<MEDIA_ID>" | grep -o "https://d1drabmetuo3qr.cloudfront.net/[^'\" ]*.mp4?[^'\"]*" | head -n 1
```

### Step 3: Stream and Save the MP4 Directly to Disk
Immediately pipe the signed URL into `curl` to download before token expiration:

```bash
STREAM_URL=$(curl -s "https://live.myvrspot.com/iframe?v=<MEDIA_ID>" | grep -o "https://d1drabmetuo3qr.cloudfront.net/[^'\" ]*.mp4?[^'\"]*" | head -n 1)

curl -o "Lesson_Video.mp4" "$STREAM_URL"
```

### Automated Python Script for MyVRSpot Videos
```python
import re
import requests

def download_myvrspot_video(media_id, output_filename):
    iframe_url = f"https://live.myvrspot.com/iframe?v={media_id}"
    res = requests.get(iframe_url)
    if res.status_code != 200:
        raise RuntimeError(f"Failed to access iframe: HTTP {res.status_code}")
    
    # Extract CloudFront signed MP4 link
    matches = re.findall(r'https://d1drabmetuo3qr\.cloudfront\.net/[^\'\"\s]+\.mp4\?[^\'\"\s]+', res.text)
    if not matches:
        raise ValueError("Could not find signed CloudFront stream in page source.")
    
    stream_url = matches[0].replace("&amp;", "&")
    print(f"Streaming from CloudFront: {stream_url[:60]}...")
    
    with requests.get(stream_url, stream=True) as stream_res:
        stream_res.raise_for_status()
        with open(output_filename, 'wb') as f:
            for chunk in stream_res.iter_content(chunk_size=1048576): # 1 MB chunks
                if chunk:
                    f.write(chunk)
    print(f"Successfully saved {output_filename}")

# Example:
# download_myvrspot_video("MjgxNGFhYmQzODAwNGQxZGU4YmE1MWUxZTIyZDc4MWM", "Video_1_Review_of_Inverses.mp4")
```

---

## 4. Playbook C: YouTube Supplementary Video Handling

When the teacher embeds third-party lessons (e.g., Mario's Math Tutoring):
- Extract the 11-character YouTube video ID (e.g. `4XytYH35AP0`).
- Embed in the study portal using the privacy-enhanced domain:
  `https://www.youtube-nocookie.com/embed/4XytYH35AP0?autoplay=1&rel=0`
- Provide direct link: `https://www.youtube.com/watch?v=4XytYH35AP0`.
- Do not attempt to re-host large YouTube MP4s unless strictly requested for offline flight mode.

---

## 5. Directory Organization & Git Synchronization

### Mandatory File Paths
All downloaded files must be organized by course and unit under `/Volumes/Backup/Antony/HighSchool/Grade9/`:
```
/Volumes/Backup/Antony/HighSchool/Grade9/
├── Math/
│   └── AP Precalculus/
│       ├── Unit 1 - Unit Circle/
│       ├── Unit 2 - Graphing Trigonometric Functions/
│       └── Unit 3 - Inverse & Composite Trigonometric Functions/
│           └── Unit 3 Quiz-9-22/
│               ├── Unit_03_Quiz_Study_Portal.html
│               ├── Unit_03_Quiz_Master_Study_Guide.md
│               ├── Video_1_Review_of_Inverses.mp4       # Local 100% offline
│               └── Video_4_Composite_Trig_Part1.mp4     # Local 100% offline
├── Biology-Honors-V2/
├── HumanGeography/
└── Intro to Software Tech/
```

### GitHub Pages Web Mirror (`ap-precalc-streams`)
- Local clone: `/Users/anish/ap-precalc-streams/`
- Remote URL: `https://github.com/MegaAntony/ap-precalc-streams.git`
- Live URL: `https://megaantony.github.io/ap-precalc-streams/`
- **Rule for Large MP4s**: Always keep `*.mp4` in `.gitignore` inside the git repository to avoid bloating GitHub limits. PDFs and HTML portals belong in the `docs/` folder for instant cloud viewing.

---

## 6. HTML Portal Dual-Mode Player Pattern

When creating study portals for Antony, always use the **Dual-Mode Player Engine**:
1. **Local Mode (`file://`)**: Automatically selects the local `.mp4` file on disk for instantaneous playback with zero buffering.
2. **Web Mode (`https://`)**: Automatically streams via responsive YouTube embeds or the official MyVRSpot iframe player.
3. Provide switcher buttons in the theater header (`[💾 Local MP4]` vs `[🌐 Web Stream]`) so Antony has complete control regardless of network connectivity.
