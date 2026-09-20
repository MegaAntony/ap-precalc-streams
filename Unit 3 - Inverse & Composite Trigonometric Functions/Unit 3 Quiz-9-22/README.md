# 🎯 AP Precalculus: Unit 3 Quiz Complete Master Study Guide (9/22)
**Assessment Date:** Tuesday, September 22, 2026 (In-Class)  
**Target Score:** 100% A+  
**Coverage:** Lessons 1 through 3 + Trig Identity Drills (TD 23–25)  
**Quick Links:**
* 🌐 **Interactive Web Study Portal**: [Open Quiz Portal HTML](./Unit_03_Quiz_Study_Portal.html) • [Live GitHub Mirror](https://megaantony.github.io/ap-precalc-streams/quiz-9-22.html)
* 📑 **Worksheet A (Inverses)**: [Worksheet PDF](https://megaantony.github.io/ap-precalc-streams/docs/APPCU03_WkstA_EvalInvFxns.pdf) • [Answer Key PDF](https://megaantony.github.io/ap-precalc-streams/docs/APPCU03_WkstA_EvalInvFxns_Answers.pdf)
* 📑 **Worksheet B (Arc Trig)**: [Worksheet PDF](https://megaantony.github.io/ap-precalc-streams/docs/APPCU03_WkstB_EvalArcTrig.pdf) • [Answer Key PDF](https://megaantony.github.io/ap-precalc-streams/docs/APPCU03_WkstB_EvalArcTrig_Answers.pdf)
* 📑 **Worksheet C (Applications)**: [Worksheet PDF](https://megaantony.github.io/ap-precalc-streams/docs/APPCU03_WkstC_Applications.pdf) • [Answer Key PDF](https://megaantony.github.io/ap-precalc-streams/docs/APPCU03_WkstC_Applications_Answers.pdf)
* ⏰ **DeltaMath Practice 1**: [DeltaMath Portal](https://www.deltamath.com) *(Due Monday 9/21 at 11:59 PM)*

---

## 🧭 Executive Summary: What is on this Quiz?

The Unit 3 Quiz on Tuesday (9/22) tests your mastery across **4 Critical Pillars**:

| Pillar | Topic | Primary Skills Tested | Associated Worksheet | Key Videos |
| :---: | :--- | :--- | :---: | :---: |
| **1** | **General Inverses & Polynomials** | Table evaluations, composition inversions $(f \circ g)^{-1}$, horizontal line test, solving $f(x)=c$ | Worksheet A | Videos 1 & 2 |
| **2** | **Evaluating Arc Trig Functions** | Strict range restrictions on $\arcsin, \arccos, \arctan$, radian exact values, reciprocal arc functions | Worksheet B | Video 3 |
| **3** | **Composite Trig Expressions** | Cancellation rules ($\arcsin(\sin\theta)$ vs $\sin(\arcsin x)$), 4-step right triangle modeling for numeric & variable ratios | Worksheet C & Videos | Videos 4, 5, 6 |
| **4** | **Trig Identities (Drill TD 23–25)** | Double angle, sum & difference, half-angle, power-reducing formulas | Trig Ident Sheet | Daily Class Drills |

---

## 🏛️ Pillar 1: General Inverses & Function Tables (Lesson 1)

### 1. Fundamental Rules of Inverses
1. **Definition**: If $f(a) = b$, then $f^{-1}(b) = a$.
2. **Domain & Range Swapping**: $\text{Domain}(f^{-1}) = \text{Range}(f)$ and $\text{Range}(f^{-1}) = \text{Domain}(f)$.
3. **Symmetry**: The graph of $y = f^{-1}(x)$ is the reflection of $y = f(x)$ across the line $y = x$.
4. **Horizontal Line Test (HLT)**: A function $f(x)$ has an inverse that is also a function **if and only if** $f$ passes the Horizontal Line Test (i.e., $f$ is strictly **one-to-one**). If a horizontal line crosses more than once, its inverse is NOT a function unless the domain is restricted!
5. **Inversion of a Composite Function**:
   $$(f \circ g)^{-1}(x) = (g^{-1} \circ f^{-1})(x) = g^{-1}(f^{-1}(x))$$
   *(Notice the order reverses!)*

### 2. Table-Based Inverses (As seen on Worksheet A)
Given a table of $x, f(x), g(x), h(x)$:
* **To find $f(g(3))$**: Look up $g(3) = 2$, then look up $f(2) = 3$.
* **To find $h^{-1}(-2)$**: Find where the output $h(x) = -2$. The corresponding input is $x = 0$. So $h^{-1}(-2) = 0$.
* **To find $(f^{-1} \circ g^{-1})(0)$**:
  1. Find $g^{-1}(0)$: Look for $g(x) = 0 \implies x = 0$.
  2. Find $f^{-1}(0)$: Look for $f(x) = 0 \implies x = -2$.
  3. Result: $-2$.
* **To find $(f \circ g)^{-1}(4)$**:
  * Using property: $(f \circ g)^{-1}(4) = g^{-1}(f^{-1}(4))$.
  * Look up $f(x) = 4 \implies x = -4$.
  * Look up $g^{-1}(-4) \implies g(x) = -4 \implies x = -2$. Result: $-2$.

### 3. Evaluating Inverses of Polynomial Functions $f^{-1}(c)$
To find $f^{-1}(c)$ when given an equation for $f(x)$:
1. Set $f(x) = c$.
2. Subtract $c$ from both sides so the equation equals zero: $f(x) - c = 0$.
3. Factor the polynomial or use Rational Root Theorem & Synthetic Division.

* **Example 1 (Factoring)**: Let $f(x) = x^3 - 7x^2 - 8x + 5$. Find $f^{-1}(5)$.
  $$x^3 - 7x^2 - 8x + 5 = 5 \implies x^3 - 7x^2 - 8x = 0$$
  Factor out $x$:
  $$x(x^2 - 7x - 8) = 0 \implies x(x - 8)(x + 1) = 0$$
  $$\mathbf{f^{-1}(5) = 0, \; 8, \; -1}$$
  *(Note: Because $f(x)$ is not one-to-one globally, there are 3 valid pre-images!)*

* **Example 2 (Quadratic-in-Form)**: Let $k(x) = 2x^4 - 9x^2 - 1$. Find $k^{-1}(-8)$.
  $$2x^4 - 9x^2 - 1 = -8 \implies 2x^4 - 9x^2 + 7 = 0$$
  Treat as $(2u^2 - 9u + 7 = 0)$ where $u = x^2$:
  $$(2x^2 - 7)(x^2 - 1) = 0$$
  $$x^2 = 1 \implies x = \pm 1$$
  $$x^2 = \frac{7}{2} \implies x = \pm\sqrt{\frac{7}{2}} = \pm\frac{\sqrt{14}}{2}$$
  $$\mathbf{k^{-1}(-8) = -1, \; 1, \; -\frac{\sqrt{14}}{2}, \; \frac{\sqrt{14}}{2}}$$

---

## 🏛️ Pillar 2: Arc Trigonometric Functions & Strict Ranges (Lesson 2)

### 1. The Strict Range Restrictions (MUST MEMORIZE 100%)
Because $\sin(x), \cos(x), \tan(x)$ are periodic, they fail the Horizontal Line Test. To define their inverses, mathematicians strictly **restricted their domains**:

| Function | Domain (Inputs) | Strict Range (Outputs $\theta$) | Active Quadrants | Notes / Endpoint Rules |
| :--- | :---: | :---: | :---: | :--- |
| $\theta = \arcsin(x) = \sin^{-1}(x)$ | $[-1, 1]$ | $\left[-\frac{\pi}{2}, \frac{\pi}{2}\right]$ | **Quadrants I & IV** | Negative angles MUST be written as negative acute angles (e.g. $-\frac{\pi}{6}$), **NEVER** as $11\pi/6$! |
| $\theta = \arccos(x) = \cos^{-1}(x)$ | $[-1, 1]$ | $[0, \pi]$ | **Quadrants I & II** | Negative inputs yield obtuse angles in Quadrant II (e.g. $\frac{2\pi}{3}, \frac{3\pi}{4}, \frac{5\pi}{6}$). |
| $\theta = \arctan(x) = \tan^{-1}(x)$ | $(-\infty, \infty)$ | $\left(-\frac{\pi}{2}, \frac{\pi}{2}\right)$ | **Quadrants I & IV** | Open interval (vertical asymptotes at $\pm\pi/2$). |
| $\theta = \text{arccsc}(x)$ | $(-\infty, -1] \cup [1, \infty)$ | $\left[-\frac{\pi}{2}, \frac{\pi}{2}\right], \theta \neq 0$ | **Quadrants I & IV** | Same as $\arcsin(1/x)$. |
| $\theta = \text{arcsec}(x)$ | $(-\infty, -1] \cup [1, \infty)$ | $[0, \pi], \theta \neq \frac{\pi}{2}$ | **Quadrants I & II** | Same as $\arccos(1/x)$. |
| $\theta = \text{arccot}(x)$ | $(-\infty, \infty)$ | $(0, \pi)$ *(standard)* or $\left(-\frac{\pi}{2}, \frac{\pi}{2}\right)$ | **QI & QII** (or QI & QIV) | *Teacher note: Both definitions are accepted on Worksheet B!* |

### 2. Unit Circle Exact Value Drills (Worksheet B Practice)
* $\arcsin\left(\frac{1}{2}\right) = \frac{\pi}{6}$
* $\arccos(0) = \frac{\pi}{2}$
* $\arctan(1) = \frac{\pi}{4}$
* $\arccos(-1) = \pi$
* $\arcsin\left(-\frac{\sqrt{3}}{2}\right) = -\frac{\pi}{3}$
* $\arctan(\sqrt{3}) = \frac{\pi}{3}$
* $\arctan\left(-\frac{1}{\sqrt{3}}\right) = -\frac{\pi}{6}$
* $\arcsin\left(-\frac{\sqrt{2}}{2}\right) = -\frac{\pi}{4}$
* $\arccos\left(\frac{\sqrt{2}}{2}\right) = \frac{\pi}{4}$
* $\text{arcsec}(-2) \implies \cos\theta = -\frac{1}{2}$ in QII $\implies \theta = \frac{2\pi}{3}$
* $\text{arccsc}(\sqrt{2}) \implies \sin\theta = \frac{\sqrt{2}}{2}$ in QI $\implies \theta = \frac{\pi}{4}$
* $\text{arcsec}\left(-\frac{2}{\sqrt{3}}\right) \implies \cos\theta = -\frac{\sqrt{3}}{2}$ in QII $\implies \theta = \frac{5\pi}{6}$

> [!CAUTION]
> **Common Trap Alert:** $\arcsin\left(-\frac{1}{2}\right) \neq \frac{11\pi}{6}$! In AP Precalculus, the range of $\arcsin$ is $\left[-\frac{\pi}{2}, \frac{\pi}{2}\right]$. Writing $\frac{11\pi}{6}$ or $\frac{7\pi}{6}$ will result in zero points. You MUST write $-\frac{\pi}{6}$.

---

## 🏛️ Pillar 3: Composite Trig Expressions (Lesson 3)

### 1. Inverse on the Inside: $f(f^{-1}(x))$
When the trig function is on the outside:
$$\sin(\arcsin(x)) = x \quad \text{for all } x \in [-1, 1]$$
$$\cos(\arccos(x)) = x \quad \text{for all } x \in [-1, 1]$$
$$\tan(\arctan(x)) = x \quad \text{for all } x \in (-\infty, \infty)$$
* Example: $\sin(\arcsin(0.4)) = 0.4$
* Example: $\sin(\arcsin(1.5)) =$ **Undefined** (because $1.5 \notin [-1, 1]$).

### 2. Inverse on the Outside: $f^{-1}(f(\theta))$ (THE BIGGEST TRAP!)
$$\arcsin(\sin(\theta)) = \theta \quad \textbf{ONLY if } \theta \in \left[-\frac{\pi}{2}, \frac{\pi}{2}\right]$$
$$\arccos(\cos(\theta)) = \theta \quad \textbf{ONLY if } \theta \in [0, \pi]$$
$$\arctan(\tan(\theta)) = \theta \quad \textbf{ONLY if } \theta \in \left(-\frac{\pi}{2}, \frac{\pi}{2}\right)$$

If $\theta$ is **outside** the restricted range, follow these **2 Steps**:
1. Evaluate the inside trig function to get a numerical ratio.
2. Evaluate the outside inverse function using the strict range restrictions!

* **Case 1**: Evaluate $\arcsin\left(\sin\left(\frac{5\pi}{6}\right)\right)$
  * Step 1: $\sin\left(\frac{5\pi}{6}\right) = \frac{1}{2}$.
  * Step 2: $\arcsin\left(\frac{1}{2}\right) = \mathbf{\frac{\pi}{6}}$ (in Quadrant I).
  * *Note: $\frac{5\pi}{6} \neq \frac{\pi}{6}$! The functions DO NOT just cancel out.*

* **Case 2**: Evaluate $\arccos\left(\cos\left(\frac{7\pi}{4}\right)\right)$
  * Step 1: $\cos\left(\frac{7\pi}{4}\right) = \frac{\sqrt{2}}{2}$ (Quadrant IV).
  * Step 2: $\arccos\left(\frac{\sqrt{2}}{2}\right) = \mathbf{\frac{\pi}{4}}$ (must be in $[0, \pi]$).

* **Case 3**: Evaluate $\arcsin\left(\sin\left(\frac{4\pi}{3}\right)\right)$
  * Step 1: $\sin\left(\frac{4\pi}{3}\right) = -\frac{\sqrt{3}}{2}$.
  * Step 2: $\arcsin\left(-\frac{\sqrt{3}}{2}\right) = \mathbf{-\frac{\pi}{3}}$.

### 3. Mixed Numeric Composites (Right Triangle Method)
To evaluate expressions like $\cos\left(\arcsin\left(\frac{3}{5}\right)\right)$ or $\tan\left(\arccos\left(-\frac{5}{13}\right)\right)$:
1. Set $\theta = \text{inside arc function}$.
2. Draw a right triangle in the appropriate quadrant:
   * For positive inputs $\implies$ Quadrant I.
   * For $\arcsin(-)$ or $\arctan(-) \implies$ Quadrant IV (angle is negative).
   * For $\arccos(-) \implies$ Quadrant II.
3. Label the two known sides (Opposite, Adjacent, Hypotenuse) and use $a^2 + b^2 = c^2$ to find the third side.
4. Read the outer trig function from the triangle.

* **Example 1**: $\cos\left(\arcsin\left(\frac{3}{5}\right)\right)$
  * Let $\theta = \arcsin(3/5) \implies \sin\theta = 3/5$ (QI).
  * $\text{Opp} = 3$, $\text{Hyp} = 5 \implies \text{Adj} = \sqrt{5^2 - 3^2} = 4$.
  * $\cos\theta = \frac{\text{Adj}}{\text{Hyp}} = \mathbf{\frac{4}{5}}$.

* **Example 2**: $\tan\left(\arccos\left(-\frac{5}{13}\right)\right)$
  * Let $\theta = \arccos(-5/13) \implies \theta \in \text{Quadrant II}$.
  * In QII, $\cos\theta = -5/13 \implies \text{Adj} = -5$, $\text{Hyp} = 13$.
  * $\text{Opp} = \sqrt{13^2 - (-5)^2} = \sqrt{169 - 25} = 12$ (positive in QII).
  * $\tan\theta = \frac{\text{Opp}}{\text{Adj}} = \frac{12}{-5} = \mathbf{-\frac{12}{5}}$.

### 4. Algebraic Variable Composites (Right Triangle Modeling)
When expressions have variable $x$, assume $x$ is in the principal domain where the triangle exists:

* **Example A**: Write $\cos(\arcsin(x))$ as an algebraic expression in $x$.
  1. Let $\theta = \arcsin(x) = \arcsin(x/1) \implies \sin\theta = \frac{x}{1}$.
  2. Draw right triangle: $\text{Opposite} = x$, $\text{Hypotenuse} = 1$.
  3. By Pythagorean theorem: $\text{Adjacent} = \sqrt{1^2 - x^2} = \sqrt{1 - x^2}$.
  4. $\cos\theta = \frac{\text{Adj}}{\text{Hyp}} = \mathbf{\sqrt{1 - x^2}}$.

* **Example B**: Write $\tan\left(\arccos\left(\frac{x}{4}\right)\right)$ as an algebraic expression.
  1. Let $\theta = \arccos(x/4) \implies \cos\theta = \frac{x}{4}$.
  2. $\text{Adjacent} = x$, $\text{Hypotenuse} = 4$.
  3. $\text{Opposite} = \sqrt{4^2 - x^2} = \sqrt{16 - x^2}$.
  4. $\tan\theta = \frac{\text{Opp}}{\text{Adj}} = \mathbf{\frac{\sqrt{16 - x^2}}{x}}$.

* **Example C**: Write $\csc(\arctan(3x))$ as an algebraic expression.
  1. Let $\theta = \arctan(3x) = \arctan(3x/1) \implies \tan\theta = \frac{3x}{1}$.
  2. $\text{Opposite} = 3x$, $\text{Adjacent} = 1$.
  3. $\text{Hypotenuse} = \sqrt{1^2 + (3x)^2} = \sqrt{1 + 9x^2}$.
  4. $\csc\theta = \frac{\text{Hyp}}{\text{Opp}} = \mathbf{\frac{\sqrt{1 + 9x^2}}{3x}}$.

---

## 🏛️ Pillar 4: Daily Trig Drills Identity Bank (TD 23–25)

Starting Monday (9/21), the daily quizzes include the newly introduced formulas. Commit these to memory:

### 1. Double-Angle Formulas
$$\sin(2\theta) = 2\sin\theta\cos\theta$$
$$\cos(2\theta) = \cos^2\theta - \sin^2\theta = 2\cos^2\theta - 1 = 1 - 2\sin^2\theta$$
$$\tan(2\theta) = \frac{2\tan\theta}{1 - \tan^2\theta}$$

### 2. Sum and Difference Formulas
$$\sin(u \pm v) = \sin u \cos v \pm \cos u \sin v$$
$$\cos(u \pm v) = \cos u \cos v \mp \sin u \sin v \quad \text{(Notice sign flips!)}$$
$$\tan(u \pm v) = \frac{\tan u \pm \tan v}{1 \mp \tan u \tan v}$$

### 3. Half-Angle Formulas
$$\sin\left(\frac{u}{2}\right) = \pm\sqrt{\frac{1 - \cos u}{2}}$$
$$\cos\left(\frac{u}{2}\right) = \pm\sqrt{\frac{1 + \cos u}{2}}$$
$$\tan\left(\frac{u}{2}\right) = \frac{1 - \cos u}{\sin u} = \frac{\sin u}{1 + \cos u} = \pm\sqrt{\frac{1 - \cos u}{1 + \cos u}}$$
*(Note: $\pm$ sign depends on which quadrant $u/2$ lies in!)*

### 4. Power-Reducing Formulas
$$\sin^2 u = \frac{1 - \cos(2u)}{2}$$
$$\cos^2 u = \frac{1 + \cos(2u)}{2}$$
$$\tan^2 u = \frac{1 - \cos(2u)}{1 + \cos(2u)}$$

---

## 📹 Video Study Playlist (Chronological Order)

Watch or review these 6 lesson videos to cover 100% of the quiz concepts:

| # | Lesson & Title | Topics | Links |
| :-: | :--- | :--- | :--- |
| **1** | **Unit 3 Lesson 1: Review of Inverses** | Algebra inverse functions, HLT, domain/range swap | [MyVRSpot](https://live.myvrspot.com/iframe?v=MjgxNGFhYmQzODAwNGQxZGU4YmE1MWUxZTIyZDc4MWM) • [Direct MP4](https://d1drabmetuo3qr.cloudfront.net/MjgxNGFhYmQzODAwNGQxZGU4YmE1MWUxZTIyZDc4MWM.midres.mp4?Expires=1789532248&Signature=q8U5RB755V1hLtE0CtjXzu3TZ9hmjcI9bhniMxPyFC-TH7CW-8qsvg46PNc1BYjTbMf31zQr1b44Ad7~Dd~SvaEXDBXg8XVOA42mzfSwp9P-ca60p~86~kGI8QSuExNZGKDvt9v~zw4leqQGSslXjrD-p2e5Z1ntw9NqOyp9kTQPQT7094kx4ivtPIU~a7~Vfj6OQjdQ9OT4Hj8eiBIgCvXiPuGp9Vqd-U0pEq81OO8oD~5iTI9x9NclJ52HazjUvkI3tZEODAeXV12xUvpbaFN2J1URcXhq6T9KDRYvTmPIpmtptD0W8a1SHFvvIeGZ7w8pCl2U7ji8QNtijEqnug__&Key-Pair-Id=APKAI62FB7DDTEKY56BA) |
| **2** | **Unit 3 Lesson 1: Rational Zero Test** | Synthetic division, factoring polynomials for $f^{-1}(c)$ | [MyVRSpot](https://live.myvrspot.com/iframe?v=fNDI2NjFhY2RjMjUyOGFhMGViZjA3MzZlNmZjZDcyMWQ) • [Direct MP4](https://d1drabmetuo3qr.cloudfront.net/4XytYH35AP0.mp4?Expires=1789532248&Signature=CEEtDJzh0BcUubXLbAp1tXr48BmE8HSz03SmbKDkMbMmgKKE7D~ljZA-QhSsjxnK3Fy0HSJ5~kKJ9--W4OepTul0e3wSOi1dgZDVa~-UJ5Y6CQ0XwnSXP~Z4ERQSpw5hC39fw5irJd84o9n~WqJopb9yTitjUiVDSC5XQTBhZ~36rs5GlllFgAiWTDnXaSraRx~VCh0Z379YhBKPB2pqBVGVn~uYVL5yoI6bicUQe5BANqRZZ-ACnrPPmAIFt5Epc2cy3xjj4vMenmuBMA14KkhzcuxVu7W66nc~VedhJKh7vIml5IwTyJAHHBXAs9dNM0wUaEkJ6TiUCY5OjetWeA__&Key-Pair-Id=APKAI62FB7DDTEKY56BA) |
| **3** | **Unit 3 Lesson 2: Evaluating Arctrig** | Exact unit circle arc values, strict quadrant restrictions | [MyVRSpot](https://live.myvrspot.com/iframe?v=fMjI5MmRjNmNiMDRmOTE0OTljMTA2ODRkZmViOGU1MDE) • [Direct MP4](https://d1drabmetuo3qr.cloudfront.net/8oDUbIYDpno.mp4?Expires=1789532249&Signature=tvUoyT1cFRQ0QzIz6TlDDBMfbHReDVNgNxxAUrOqr6kLRc6k-H9lG1CbOe8kJk3VfwSs~t1mIakn3EKoMjYK0ro46o8uYrSsE2fU3WUGg0MfbTqr0TrnMq7F1Bga-1MZ3UKxspBE1dkeiuwoRSpazRULJ-kwc3C-zSD0dkFz2-mNvq3npnl3ZdWaSnqK8ElF1jwzSbg2famv9Szu15qY61Y0ya6YAWRPFKzL0ripGKIGy1PSWkik1ATNn8i1Uei2U~GOY4w~EbSUro9vpnm2GBbwWR2QV3EJf6ZPynvERUks5omILx420Ngb5mQDkYuGMYOgCbbhXsHvHU9YCtbwpw__&Key-Pair-Id=APKAI62FB7DDTEKY56BA) |
| **4** | **Unit 3 Lesson 3: Composite Trig (Part 1)** | Cancellation rules, out-of-range cases | [MyVRSpot](https://live.myvrspot.com/iframe?v=MTFkYmY2Y2M3ZjAyOGM3MzU1YjI4YjMxYmRlMmU3ZDI) • [Direct MP4](https://d1drabmetuo3qr.cloudfront.net/MTFkYmY2Y2M3ZjAyOGM3MzU1YjI4YjMxYmRlMmU3ZDI.highres.mp4?Expires=1789532249&Signature=N0sQJNkp5nMBgcyrHOaLXPqj9pkmAV~lRp3HvQUCOAaFnZyrplAAeLLCyRnHI87xL-fNP0rFac4m-fPqUJ53I8Hw8yy0F0RDQLSHe~buQqX9UYAy0ynIJF6hgKksuEneFQSEFqEupCNf7Us4nSe~7X5d1OTynlALaVKBTka0lDh59FuYT33UY-sA8O0guBPqpoNU2QcmdNq4S4By5WPUkyqNOGkEbaKhFBrrnSGQAf41rnuRF2v~yXrNiT0j8siObUKHJtLKwNT6NwmKhlUOiYVUUHgYreVoqq9XRPch0-y9FREQGEuYg23AtoNRCa8bQwe8tQsd2jvX9CgIwTrpFg__&Key-Pair-Id=APKAI62FB7DDTEKY56BA) |
| **5** | **Unit 3 Lesson 3: Numeric Composites (Part 2)** | Numeric ratios, right triangle evaluation | [MyVRSpot](https://live.myvrspot.com/iframe?v=fOWU3MDJiODA5NWY3NDE5M2MzOWYzNTZiOTgxMWU0M2I) • [YouTube Video](https://www.youtube.com/watch?v=FttVzfrk5L8) |
| **6** | **Unit 3 Lesson 3: Variable Ratios (Part 3)** | Algebraic triangle modeling with $x$ | [MyVRSpot](https://live.myvrspot.com/iframe?v=fMjY3MmM4OTQ5YmI4NzY3ZjY0ZTJmNzhlMjEyNzRhMjY) • [YouTube Video](https://www.youtube.com/watch?v=OLCNPVCMQPw) |

---

## 📝 Practice Quiz Simulation (Self-Test with Solutions)

Test yourself on these 10 AP-style questions without looking at the solutions first:

### Questions
1. If $g(x) = x^3 + 3x^2 - 4x - 10$, find all values of $g^{-1}(2)$.
2. The table gives values of $f(x)$ and $g(x)$:
   * $x = \{-2, -1, 0, 1, 2\}$
   * $f(x) = \{0, -1, 2, -4, 3\}$
   * $g(x) = \{-4, 4, 0, 3, -2\}$
   * Evaluate $(f \circ g)^{-1}(3)$.
3. Evaluate $\arcsin\left(-\frac{\sqrt{3}}{2}\right)$ in exact radians.
4. Evaluate $\arccos\left(-\frac{\sqrt{2}}{2}\right)$ in exact radians.
5. Evaluate $\text{arcsec}(-2)$ in exact radians.
6. Evaluate $\arcsin\left(\sin\left(\frac{5\pi}{6}\right)\right)$.
7. Evaluate $\arccos\left(\cos\left(-\frac{\pi}{3}\right)\right)$.
8. Evaluate $\tan\left(\arccos\left(-\frac{5}{13}\right)\right)$.
9. Write $\sin(\arccos(2x))$ as an algebraic expression in $x$.
10. Write $\tan\left(\arcsin\left(\frac{x}{\sqrt{x^2 + 25}}\right)\right)$ as an algebraic expression in $x$.

---

### Step-by-Step Solutions
1. **$g(x) = 2 \implies x^3 + 3x^2 - 4x - 12 = 0$.**
   * Factor by grouping: $x^2(x + 3) - 4(x + 3) = (x^2 - 4)(x + 3) = (x - 2)(x + 2)(x + 3) = 0$.
   * **Answer: $x = -3, -2, 2$**.
2. **$(f \circ g)^{-1}(3) = g^{-1}(f^{-1}(3))$.**
   * From table, $f(x) = 3 \implies x = 2$.
   * Now find $g^{-1}(2) \implies$ look for $g(x) = 2$. If not present or check table: from Worksheet A table, $g(3) = 2 \implies g^{-1}(2) = 3$.
   * **Answer: 3**.
3. $\arcsin(-\sqrt{3}/2)$ must be in Quadrant IV as a negative acute angle.
   * $\sin(-\pi/3) = -\sqrt{3}/2 \implies \mathbf{-\frac{\pi}{3}}$.
4. $\arccos(-\sqrt{2}/2)$ must be in Quadrant II.
   * Reference angle $\pi/4 \implies \pi - \pi/4 = \mathbf{\frac{3\pi}{4}}$.
5. $\text{arcsec}(-2) \implies \cos\theta = -1/2$ in Quadrant II.
   * $\theta = \pi - \pi/3 = \mathbf{\frac{2\pi}{3}}$.
6. $\arcsin(\sin(5\pi/6)) = \arcsin(1/2) = \mathbf{\frac{\pi}{6}}$. *(Not $5\pi/6$!)*
7. $\cos(-\pi/3) = \cos(\pi/3) = 1/2$. Then $\arccos(1/2) = \mathbf{\frac{\pi}{3}}$.
8. Let $\theta = \arccos(-5/13)$ in QII. $\text{Adj} = -5, \text{Hyp} = 13 \implies \text{Opp} = 12$.
   * $\tan\theta = \frac{\text{Opp}}{\text{Adj}} = \mathbf{-\frac{12}{5}}$.
9. Let $\theta = \arccos(2x/1)$. $\text{Adj} = 2x, \text{Hyp} = 1 \implies \text{Opp} = \sqrt{1 - (2x)^2} = \sqrt{1 - 4x^2}$.
   * $\sin\theta = \mathbf{\sqrt{1 - 4x^2}}$.
10. Let $\theta = \arcsin\left(\frac{x}{\sqrt{x^2+25}}\right)$.
    * $\text{Opp} = x$, $\text{Hyp} = \sqrt{x^2+25}$.
    * $\text{Adj} = \sqrt{(\sqrt{x^2+25})^2 - x^2} = \sqrt{x^2+25 - x^2} = \sqrt{25} = 5$.
    * $\tan\theta = \frac{\text{Opp}}{\text{Adj}} = \mathbf{\frac{x}{5}}$.

---

## 🗓️ 2-Day Hour-by-Hour Study Schedule (100% Score Protocol)

### Sunday, September 20, 2026 (Concept Mastery & Video Review)
* **2:00 PM – 3:15 PM**: Watch **Videos 1 & 2** (Inverses & Rational Zero Test).
  * Work through Worksheet A problems #1–15 on paper.
  * Check answers against [Worksheet A Answer Key](https://megaantony.github.io/ap-precalc-streams/docs/APPCU03_WkstA_EvalInvFxns_Answers.pdf).
* **3:30 PM – 4:45 PM**: Watch **Video 3** (Evaluating Arctrig Functions).
  * Work through Worksheet B problems #1–18.
  * Memorize the restricted ranges: $\arcsin \in [-\pi/2, \pi/2]$, $\arccos \in [0, \pi]$, $\arctan \in (-\pi/2, \pi/2)$.
  * Verify against [Worksheet B Answer Key](https://megaantony.github.io/ap-precalc-streams/docs/APPCU03_WkstB_EvalArcTrig_Answers.pdf).
* **5:00 PM – 6:15 PM**: Watch **Videos 4, 5, 6** (Composite Trig Expressions & Variable Ratios).
  * Practice the 4-step right triangle modeling technique for both numeric and algebraic ratios.
* **7:30 PM – 8:30 PM**: Memorize Trig Identities (Double Angle, Sum/Difference, Half-Angle, Power-Reducing).
  * Write them out on a blank sheet 3 times without looking!

### Monday, September 21, 2026 (Assignment & Drill Finalization)
* **During School**: Pay close attention during class drill **TD 23**. Note any question types the teacher emphasizes.
* **4:30 PM – 6:00 PM**: Complete **DeltaMath – Unit 3: Practice 1** (Due at 11:59 PM).
  * Ensure 100% completion and rework any missed problem until you understand the underlying concept.
* **6:30 PM – 7:30 PM**: Solve Worksheet C word problems (Angle of elevation, descent, ladder).
  * Check with [Worksheet C Answer Key](https://megaantony.github.io/ap-precalc-streams/docs/APPCU03_WkstC_Applications_Answers.pdf).
* **7:45 PM – 8:30 PM**: Take the **10-Question Practice Quiz Simulation** in this guide under timed exam conditions (20 minutes).
* **8:30 PM – 9:00 PM**: Final review of the **Pillar 2 & 3 Trap Alerts** (out-of-bounds arc functions, negative QIV angles).
* **Good night's rest**: Sleep by 10:00 PM so your recall speed is peak tomorrow!

---

*This guide is prepared specifically for Antony's AP Precalculus class at South Forsyth High School. All files and videos are permanently accessible without school login.*
