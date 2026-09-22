# The Grade Ledger

An interactive, single-page data visualization that models a decision every student faces: **how will my midterm, assignment, and final exam scores add up — and what does that do to my overall GPA?**

Built for the *Build an Interactive Data Visualization* mission (Google AI Professional Certificate track).

**Live demo:** https://prince12raj.github.io/Google_Build-an-Interactive-Data-Visualization/

## What it does

Three sliders model the variables that actually determine a course grade:

| Variable | Weight |
|---|---|
| Midterm score | 30% |
| Assignments & quizzes average | 30% |
| Final exam score | 40% |

Moving any slider instantly recalculates and redraws:

- Your **class percentage and letter grade** (standard 4.0 scale, A through F with +/− steps)
- A **stacked bar chart** showing exactly how much each component contributes to the total
- Your **projected overall CGPA**, using an optional fold-out section where you can enter your current CGPA, credits completed, and this course's credit hours — with a delta showing whether the course pulls your CGPA up or down

Everything updates live with no submit button, and nothing is saved or sent anywhere — the whole thing runs client-side in the page.

## Tech

- Plain HTML, CSS, and vanilla JavaScript — no frameworks, no build step, no dependencies to install
- Google Fonts (Lora + JetBrains Mono) loaded via `<link>`
- Charts drawn as inline SVG
- Responsive layout, dark-mode aware (follows your system's light/dark setting), keyboard-accessible sliders

## Running it locally

Just open `index.html` in a browser — no server or build step required.

## Deployment

Hosted on GitHub Pages, deployed from the `main` branch, `/(root)` folder.

## Customizing

The grading weights (30/30/40) and the letter-grade cutoffs are defined near the top of the `<script>` block in `index.html` (`WEIGHTS` object and the `gradeTier()` function) — edit those to match your own school's grading scale.
