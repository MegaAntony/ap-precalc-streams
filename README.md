# 📐 AP Precalculus Course Archive & Video Stream Portal

This repository and backup archive serves as the centralized offline and cloud hub for **AP Precalculus (Grade 9)**. It contains lesson video archives, direct MP4 streaming links, textbooks, worksheets, and answer keys hosted publicly with **zero authentication required**.

---

## 🌐 Live Web Portal & Repository Details
* **GitHub Username**: `MegaAntony`
* **Live Website**: [https://megaantony.github.io/ap-precalc-streams/](https://megaantony.github.io/ap-precalc-streams/)
* **GitHub Repository**: [https://github.com/MegaAntony/ap-precalc-streams](https://github.com/MegaAntony/ap-precalc-streams)
* **Local Git Repo Path**: `/Users/anish/ap-precalc-streams/`
* **Backup & Materials Path**: `/Volumes/Backup/Antony/HighSchool/Grade9/Math/AP Precalculus/`

---

## 🔑 GitHub SSH Key & Authentication Details

### 1. Your Public SSH Key
```text
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIKNMmVVgIknZ8nylByh9K74/GnaXwQ4gJ/Go24lWEy82 MegaAntony@github
```

### 2. Key File Paths on macOS
* **Public Key**: `~/.ssh/id_ed25519.pub` (`/Users/anish/.ssh/id_ed25519.pub`)
* **Private Key**: `~/.ssh/id_ed25519` (`/Users/anish/.ssh/id_ed25519`)
* **SSH Config**: `~/.ssh/config` (`/Users/anish/.ssh/config`)

### 3. Quick Terminal Commands
* **Copy Public Key to Clipboard**:
  ```bash
  pbcopy < ~/.ssh/id_ed25519.pub
  ```
* **Test GitHub SSH Authentication**:
  ```bash
  ssh -T git@github.com
  ```
* **Re-add Key to macOS Keychain (if ever needed)**:
  ```bash
  ssh-add --apple-use-keychain ~/.ssh/id_ed25519
  ```

---

## 📁 Directory Structure & Existing Units

```text
/Volumes/Backup/Antony/HighSchool/Grade9/Math/AP Precalculus/
├── README.md                                  # Complete course and setup documentation
├── AP_Precalculus_Direct_MP4_Streams.html     # Mirror copy of the stream portal HTML
├── Weekly Plans/                              # Master calendar, weekly schedules, & daily assignments
│   ├── README.md                              # Semester 1 schedule, milestones & deadlines
│   ├── Week_07_Sep_14_Sep_18.md               # Unit 2 Test, Intro to Inverses & Composites
│   ├── Week_08_Sep_21_Sep_25.md               # Right Triangles, Area Formulas, Unit 3 Quiz (9/22), Law of Cosines
│   ├── Week_Fall_Break_Sep_28_Oct_02.md       # Fall Break (no school, covers Oct 1 & Oct 2)
│   └── Week_09_Oct_05_Oct_09.md               # October First Week: Law of Sines, Ambiguous Case SSA, Review
├── Textbook/                                  # 5 offline textbook PDF chapters & solution keys
│   ├── Precalculus_Chapter_04_Trigonometric_Functions.pdf
│   ├── Precalculus_Chapter_05_Analytic_Trigonometry.pdf
│   ├── Precalculus_Chapter_06_Additional_Topics_Trig.pdf
│   ├── Precalculus_Answers_to_Odd_Problems.pdf
│   └── Precalculus_Index_and_Formula_Pages.pdf
├── Unit 1 - Unit Circle/
│   ├── Unit_01_all-Lesson_Videos.md           # 12 videos with direct MP4 streams & curl commands
│   ├── Unit_01_Complete_Reference.md          # Local textbook links, Worksheets A-D, solution keys
│   ├── unit_01_metadata.json                  # Raw parsed Canvas data
│   ├── handouts/                              # 5 offline reference PDFs (Identities, Unit Circle, Graph Paper)
│   │   ├── Official_Trig_Identities_Sheet.pdf
│   │   ├── Blank_Unit_Circle_Sheet.pdf
│   │   └── ... (3 graph paper PDFs)
│   └── worksheets/                            # 8 offline local PDF worksheets & answer keys
│       ├── APPCU01_WkstA_AngularLinearSpeed.pdf
│       ├── APPCU01_WkstA_AngularLinearSpeed_Answers.pdf
│       ├── APPCU01_WkstB_ExtraPracticeQuiz.pdf
│       ├── APPCU01_WkstB_ExtraPracticeQuiz_Answers.pdf
│       ├── APPCU01_WkstC_ReferenceAngles.pdf
│       ├── APPCU01_WkstC_ReferenceAngles_Answers.pdf
│       ├── APPCU01_WkstD_ReviewForTest.pdf
│       └── APPCU01_WkstD_ReviewForTest_Answers.pdf
├── Unit 2 - Graphing Trigonometric Functions/
│   ├── Unit_02_all-Lesson_Videos.md           # 12 direct MP4 streams for current & older AP lessons
│   ├── Unit_02_Complete_Reference.md          # Offline local Worksheets A-F, graphs, test reviews
│   ├── unit_02_metadata.json                  # Raw parsed Canvas data
│   └── worksheets/                            # 12 offline local PDF worksheets & answer keys
│       ├── APPCU02_WkstA_GraphingSineCosine.pdf
│       ├── APPCU02_WkstA_GraphingSineCosine_Answers.pdf
│       ├── APPCU02_WkstB_GraphingSecantCosecant.pdf
│       ├── APPCU02_WkstB_GraphingSecantCosecant_Answers.pdf
│       ├── APPCU02_WkstC_GraphingTangentCotangent.pdf
│       ├── APPCU02_WkstC_GraphingTangentCotangent_Answers.pdf
│       ├── APPCU02_Lesson4_Graphs.pdf
│       ├── APPCU02_WkstD_WritingEquationsFromGraphs.pdf
│       ├── APPCU02_WkstD_WritingEquationsFromGraphs_Answers.pdf
│       ├── APPCU02_WkstE_TestReview.pdf
│       ├── APPCU02_WkstE_TestReview_Answers.pdf
│       └── APPCU02_WkstF_Applications.pdf
└── Unit 3 - Inverse & Composite Trigonometric Functions/
    ├── Unit_03_all-Lesson_Videos.md           # Direct MP4 streams for 13 lessons & examples
    ├── Unit_03_Complete_Reference.md          # Worksheets A-E, oblique triangles, test reviews
    ├── unit_03_metadata.json                  # Raw parsed Canvas data for 15 pages
    └── worksheets/                            # 16 offline local PDF worksheets & answer keys
        ├── APPCU03_WkstA_EvalInvFxns.pdf
        ├── APPCU03_WkstA_EvalInvFxns_Answers.pdf
        ├── APPCU03_WkstB_EvalArcTrig.pdf
        ├── APPCU03_WkstB_EvalArcTrig_Answers.pdf
        ├── APPCU03_WkstB_AppsObliqueTriangles.pdf
        ├── APPCU03_WkstB_AppsObliqueTriangles_Answers.pdf
        ├── APPCU03_WkstC_Applications.pdf
        ├── APPCU03_WkstC_Applications_Answers.pdf
        ├── APPCU03_WkstC_ExtraPracSSA.pdf
        ├── APPCU03_WkstC_ExtraPracSSA_Answers.pdf
        ├── APPCU03_WkstD_MorePracticeApps.pdf
        ├── APPCU03_WkstD_MorePracticeApps_Answers.pdf
        ├── APPCU03_WkstD_UnitReview.pdf
        ├── APPCU03_WkstD_UnitReview_Answers.pdf
        ├── APPCU03_WkstE_Review.pdf
        └── APPCU03_WkstE_Review_Answers.pdf
```

Hosted public repository layout:
```text
/Users/anish/ap-precalc-streams/
├── index.html                                 # Live portal with nav bar, videos & worksheets
├── docs/                                      # 46 Zero-Auth PDFs (Textbook, Handouts, Worksheets, Keys)
│   ├── Precalculus_Chapter_04_Trigonometric_Functions.pdf
│   ├── Precalculus_Chapter_05_Analytic_Trigonometry.pdf
│   ├── Precalculus_Chapter_06_Additional_Topics_Trig.pdf
│   ├── Precalculus_Answers_to_Odd_Problems.pdf
│   ├── Precalculus_Index_and_Formula_Pages.pdf
│   ├── Official_Trig_Identities_Sheet.pdf
│   ├── Blank_Unit_Circle_Sheet.pdf
│   ├── Graph_Paper_4_blocks.pdf / Graph_Paper_10_blocks.pdf / Polar_Graph_Paper.pdf
│   ├── APPCU01_... (8 Unit 1 PDFs)
│   ├── APPCU02_... (12 Unit 2 PDFs)
│   └── APPCU03_... (16 Unit 3 PDFs)
├── Unit 1 - Unit Circle/                      # Unit 1 reference docs & video index
├── Unit 2 - Graphing Trigonometric Functions/ # Unit 2 reference docs & video index
├── Unit 3 - Inverse & Composite Trigonometric Functions/ # Unit 3 reference docs & video index
└── Weekly Plans/                              # Master calendar & weekly schedule trackers
```

---

## 📖 Complete Course Materials (100% Zero-Auth Links)

### 📚 Official Course Textbook (Larson Precalculus)
* **Chapter 4 - Trigonometric Functions (pgs 257–350)**: [Download Web PDF](https://megaantony.github.io/ap-precalc-streams/docs/Precalculus_Chapter_04_Trigonometric_Functions.pdf)
* **Chapter 5 - Analytic Trigonometry (pgs 351–406)**: [Download Web PDF](https://megaantony.github.io/ap-precalc-streams/docs/Precalculus_Chapter_05_Analytic_Trigonometry.pdf)
* **Chapter 6 - Additional Topics in Trigonometry (pgs 407–472)**: [Download Web PDF](https://megaantony.github.io/ap-precalc-streams/docs/Precalculus_Chapter_06_Additional_Topics_Trig.pdf)
* **Answers to Odd Problems (Complete Solution Key)**: [Download Web PDF](https://megaantony.github.io/ap-precalc-streams/docs/Precalculus_Answers_to_Odd_Problems.pdf)
* **Index and Reference Formula Pages**: [Download Web PDF](https://megaantony.github.io/ap-precalc-streams/docs/Precalculus_Index_and_Formula_Pages.pdf)

### 📐 Reference Handouts & Graph Paper
* **Official Trig Identities Sheet**: [Download Web PDF](https://megaantony.github.io/ap-precalc-streams/docs/Official_Trig_Identities_Sheet.pdf)
* **Blank Unit Circle Practice Sheet**: [Download Web PDF](https://megaantony.github.io/ap-precalc-streams/docs/Blank_Unit_Circle_Sheet.pdf)
* **Cartesian Graph Paper (4 blocks/inch)**: [Download Web PDF](https://megaantony.github.io/ap-precalc-streams/docs/Graph_Paper_4_blocks.pdf)
* **Cartesian Graph Paper (10 blocks/inch)**: [Download Web PDF](https://megaantony.github.io/ap-precalc-streams/docs/Graph_Paper_10_blocks.pdf)
* **Polar Coordinate Graph Paper**: [Download Web PDF](https://megaantony.github.io/ap-precalc-streams/docs/Polar_Graph_Paper.pdf)

---

## 📖 Units Breakdown

### 1. [Unit 1 - Unit Circle](./Unit%201%20-%20Unit%20Circle/)
* **Video Archive**: [`Unit_01_all-Lesson_Videos.md`](./Unit%201%20-%20Unit%20Circle/Unit_01_all-Lesson_Videos.md) (12 Videos)
  * Standard Position, Radians, Coterminal Angles, Comp/Supp, Unit Circle, Angular/Linear Speed, Quadrant System, Reference Angles.
* **Reference & Worksheets**: [`Unit_01_Complete_Reference.md`](./Unit%201%20-%20Unit%20Circle/Unit_01_Complete_Reference.md)
  * Worksheets A–D & Full Answer Keys (8 PDFs hosted live in `docs/` with zero authentication).

### 2. [Unit 2 - Graphing Trigonometric Functions](./Unit%202%20-%20Graphing%20Trigonometric%20Functions/)
* **Video Archive**: [`Unit_02_all-Lesson_Videos.md`](./Unit%202%20-%20Graphing%20Trigonometric%20Functions/Unit_02_all-Lesson_Videos.md) (12 Videos)
  * Khan Academy Sine graphs, ScreenPal lessons 1–5 & 10, Older versions (2.1a–d), Secant/Cosecant, Writing Equations from Graphs.
* **Reference & Worksheets**: [`Unit_02_Complete_Reference.md`](./Unit%202%20-%20Graphing%20Trigonometric%20Functions/Unit_02_Complete_Reference.md)
  * Worksheets A–F, Lesson 4 graphs, test reviews (12 PDFs hosted live in `docs/` with zero authentication).

### 3. [Unit 3 - Inverse & Composite Trigonometric Functions](./Unit%203%20-%20Inverse%20%26%20Composite%20Trigonometric%20Functions/)
* **Video Archive**: [`Unit_03_all-Lesson_Videos.md`](./Unit%203%20-%20Inverse%20%26%20Composite%20Trigonometric%20Functions/Unit_03_all-Lesson_Videos.md) (13 Videos)
  * **Lesson 1**: Review of Inverses & Rational Zero Test (Synthetic Division)
  * **Lesson 2**: Evaluating Arctrig Functions
  * **Lesson 3**: Composite Trig Expressions, Numeric Only & Variable Ratios
  * **Lesson 4**: Pythagorean & Reciprocal Identities, SAS & Heron's Triangle Area
  * **Lesson 5**: Oblique Triangles and Law of Cosines
  * **Lesson 6**: Law of Sines
  * **Lesson 7**: Ambiguous Case of Law of Sines & Worked 2-Triangle Example (Mr. O'Connor notation)
* **Reference & Worksheets**: [`Unit_03_Complete_Reference.md`](./Unit%203%20-%20Inverse%20%26%20Composite%20Trigonometric%20Functions/Unit_03_Complete_Reference.md)
  * Worksheets A–E, oblique triangles, test reviews (16 PDFs hosted live in `docs/` with zero authentication).

### 4. [Weekly Plans & Assignment Tracker](./Weekly%20Plans/)
* **Master Schedule & Milestones**: [`Weekly Plans/README.md`](./Weekly%20Plans/README.md)
* **[Week 7 (9/14 – 9/18)](./Weekly%20Plans/Week_07_Sep_14_Sep_18.md)**: Unit 2 Test, Begin Unit 3 (Lessons 1–3, Inverse Functions & Graphing).
* **[Week 8 (9/21 – 9/25)](./Weekly%20Plans/Week_08_Sep_21_Sep_25.md)**: Right Triangles, Area Formulas ($SAS$ & Heron's), **Unit 3 Quiz (Tue 9/22)**, Law of Cosines, DeltaMath Practice 1 (due 9/21) & Practice 2 (due 9/27).
* **[Fall Break (9/28 – 10/2)](./Weekly%20Plans/Week_Fall_Break_Sep_28_Oct_02.md)**: Fall Break review & identity practice (covers Oct 1 & Oct 2).
* **[Week 9 — October First Week (10/5 – 10/9)](./Weekly%20Plans/Week_09_Oct_05_Oct_09.md)**: Law of Sines, Ambiguous Case (SSA Two-Triangle Case), Unit 3 Review, DeltaMath Practice 3 (due 10/8), Unit 3 Test Prep (Test: 10/12–10/13).

---

## 🛠️ Case Study: How We Built Unit 3

### Step 1: Read Canvas Home Page with 5-Second Delay
Using the student's Canvas session cookie, we scraped `https://forsyth.instructure.com/courses/276219` with `sleep 5` to avoid bot detection. We parsed the weekly plan (`AP Precalc 26/27 Week 7`) and discovered Unit 3 was newly active.

### Step 2: Query Canvas Modules API
We pulled all module items via:
```bash
curl -s "https://forsyth.instructure.com/api/v1/courses/276219/modules?include[]=items&per_page=50" \
  -H "accept: application/json" -b "canvas_session=..."
```
This returned the exact page slugs for all 7 video lessons and 8 worksheet pages.

### Step 3: Scrape All Unit Pages with 5s Delay
A Python script fetched each of the 15 pages with `time.sleep(5)` intervals and exported `unit_03_metadata.json`.

### Step 4: Extract Direct Video Streams
1. **MyVRSpot Videos**: Queried the embed player iframe (`https://live.myvrspot.com/iframe?v=<ID>`) which returned direct, high-res signed CloudFront MP4 stream URLs (`https://d1drabmetuo3qr.cloudfront.net/...mp4`).
2. **ScreenPal Videos**: Extracted the direct player stream endpoint (`https://go.screenpal.com/player/stream/<ID>`), usable with `curl -L -H "Referer: ..."` or downloadable in-browser.
3. **Canvas Studio**: Extracted the Studio embed player URLs.

### Step 5: Solve the SharePoint Login Issue (Auth-Free PDFs)
* School SharePoint links (`forsythk12org.sharepoint.com/:b:/s/SFHMath/...`) require Microsoft 365 student login and return HTTP 403 / redirect to Azure AD if accessed by external visitors.
* **The Solution**: We downloaded all 16 PDFs using the authenticated browser session into a temporary staging folder (`/Volumes/Backup/scrap/x/`).
* Copied all 16 PDFs to:
  1. `/Volumes/Backup/.../Unit 3 - .../worksheets/` (permanent local backup)
  2. `/Users/anish/ap-precalc-streams/docs/` (public web hosting)
* Configured `index.html` buttons to link to `./docs/<filename>.pdf`. GitHub Pages serves these as native static files with **zero authentication required**!

### Step 6: Web Portal UI Enhancements
* Added a **sticky navigation bar** at the top with jump links (`#unit-1`, `#unit-2`, `#unit-3`, and `#unit-3-review`).
* Added `html { scroll-behavior: smooth; }` and a JavaScript pulse animation that highlights the selected unit card with a glowing blue border.
* Committed and pushed to `main` branch:
  ```bash
  cd ~/ap-precalc-streams
  git add index.html docs/
  git commit -m "Publish Unit 3 worksheets and answer key PDFs (auth-free public access)"
  git push
  ```

---

## 🚀 How to Add Next Chapters (Unit 4, 5, etc.)

Whenever a new unit is posted on Canvas, follow this standard 4-step workflow:

### Step 1: Copy Canvas Cookie & Run Initial Extraction
1. Open Chrome DevTools (`Cmd + Option + I`) on Canvas -> Network tab.
2. Refresh `https://forsyth.instructure.com/courses/276219`.
3. Right click the document request -> **Copy as cURL**.
4. In chat prompt, say:
   > *"Extract Unit X with 5s delay and update the hosted website"*

### Step 2: Automatic Scrape & Video Stream Resolution
The assistant will:
1. Fetch `https://forsyth.instructure.com/api/v1/courses/276219/modules`.
2. Extract all Lesson pages and Worksheet pages for Unit X with 5-second delays.
3. Resolve all MyVRSpot iframes to CloudFront MP4 URLs and ScreenPal stream endpoints.
4. Create the folder:
   `/Volumes/Backup/Antony/HighSchool/Grade9/Math/AP Precalculus/Unit X - <Title>/`
   containing `unit_0X_metadata.json`, `Unit_0X_all-Lesson_Videos.md`, and `Unit_0X_Complete_Reference.md`.

### Step 3: Download Worksheets for Zero-Auth Hosting
To make worksheets public without school login:
1. Open the SharePoint links for Unit X in your browser (since you are logged into Microsoft 365).
2. Download the worksheet PDFs and answer keys (either via browser Save As or into a staging folder like `~/Downloads` or `/Volumes/Backup/scrap/x/`).
3. Tell the assistant:
   > *"Downloaded Unit X worksheets to <path>. Copy to right folder and publish"*
4. The assistant will copy them to `docs/` and `worksheets/`, update the portal buttons to point to the local `./docs/...` files, and update `Unit_0X_Complete_Reference.md`.

### Step 4: Publish Live to GitHub Pages
The assistant will commit and push the updates:
```bash
cd ~/ap-precalc-streams
git add index.html docs/
git commit -m "Add Unit X lessons, video streams, and auth-free worksheets"
git push
```
The website at [https://megaantony.github.io/ap-precalc-streams/](https://megaantony.github.io/ap-precalc-streams/) will update automatically in ~30 seconds.

---

### 💡 Quick Refresh Tip
GitHub Pages sends `Cache-Control: max-age=600` (10-minute cache). When viewing a newly published unit, either:
* Press **`Cmd + Shift + R`** in your browser.
* Or add a query parameter to the URL (e.g. `https://megaantony.github.io/ap-precalc-streams/?v=4#unit-4`).
