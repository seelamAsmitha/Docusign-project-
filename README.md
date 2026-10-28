# DocuSign Clone: QA Bug Hunt, Triage & Reporting

A structured QA pass on a DocuSign clone, comparing it against the real DocuSign application. I found, categorised and prioritised 60 defects across UI fidelity, functional flows, accessibility, hard-coded data and page metadata.

Note: This was completed as a QA Intern take-home assessment. The client's login details and the original assignment brief are intentionally not included in this repository.

## Highlights

- 60 bugs logged, one bug per row, each with reproduction steps, expected vs actual behaviour, evidence links, browser and OS, viewport and reproducibility.
- Severity triaged from P1 to P4 using a defined scale: Blocker, Critical, Major, Minor, Trivial.
- Pixel-level comparison against the original app at a fixed 1280x960 viewport in Chrome.
- Coverage of the Home dashboard, Templates module, global header and footer, plus page metadata and accessibility markup.

## Results at a Glance

| Severity | Meaning | Count |
|---|---|---|
| P1 | Critical | 2 |
| P1 / P2 | Borderline, needs product call | 1 |
| P2 | Major | 10 |
| P3 | Minor | 21 |
| P4 | Trivial | 25 |
| Unrated | Severity to be assigned | 1 |
| Total | | 60 |

| Category | Count |
|---|---|
| UI / Pixel | 20 |
| Functional | 14 |
| Accessibility / Markup | 12 |
| Hard-coded data / Metadata | 9 |
| UI / Mobile | 3 |
| Architecture / Other | 2 |

## Top 5 Bugs I Would Fix First

1. BUG-045: Signature field cannot be moved, resized or deleted after placement. This breaks the core Prepare flow, so a sender cannot correct a misplaced field.
2. BUG-047: Unexpected third-party script (/grade.js) in the base page shell. An external script that the original does not load is a trust and data-handling concern.
3. BUG-048: Tech stack differs from the original app. This affects how faithfully the clone behaves and how it can be maintained.
4. BUG-001: Home two-column row overflows its container at 1280px. The main screen is visibly misaligned at the reference viewport.
5. BUG-004: Start an agreement button is disabled in the empty state. The primary call to action on the landing screen does nothing.

## Method

1. Fixed the environment: Chrome, 1280x960, 100% zoom, and recorded browser and OS version.
2. Walked the happy path on the original and the clone side by side.
3. Ran a pixel pass per screen: spacing, colour, font weight, icon size and states.
4. Ran a functional pass per module: validation, navigation, empty states and error handling.
5. Audited hard-coded and seeded data, plus page metadata and accessibility markup.
6. Triaged at the end: severity, de-duplication, and cross-references between related bugs.

## Tools Used

Google Chrome DevTools, side-by-side comparison with the original DocuSign app, screenshots and screen recordings, and a spreadsheet bug tracker.

## Repository Structure

- README.md: project overview
- bug_tracker_Asmita_Reddy_Seelam.xlsx: full bug tracker with all 60 bugs
- docs/summary_note.md: one-page summary of findings
- evidence/: annotated screenshots and recordings named BUG-00X_module_short-slug

## Skills Demonstrated

Manual testing, UI and pixel-level comparison, functional and edge-case testing, bug reporting, severity triage, accessibility review, DevTools debugging, test documentation, attention to detail.

## What I Learned

- Writing reproduction steps that a developer can follow without asking questions.
- Separating severity (user impact) from how annoying a bug feels.
- Grouping bugs that share a root cause and cross-referencing them instead of duplicating.
- Using DevTools to turn looks off into measurable values.

## Author

Asmita Reddy Seelam
Final year B.Tech, Artificial Intelligence and Machine Learning
Adi Shankara College of Engineering and Technology, Gudur, Tirupati

LinkedIn:  www.linkedin.com/in/asmitha-reddy-seelam-b40610300
GitHub: https://github.com/seelamAsmitha
Email: seelamasmitha7@gmail.com
