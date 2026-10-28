# Evidence

This file documents the proof behind the bugs in the tracker: annotated screenshots and screen recordings captured at the moment each bug was found.

## How evidence is organised

- Every file is named BUG-00X_module_short-slug, matching the Bug ID in the spreadsheet.
- Screenshots are annotated and show the URL bar so the screen is easy to recognise.
- Screen recordings are used for anything involving a sequence of steps or timing.
- Side-by-side comparisons show the original DocuSign and the clone at the same viewport.

Example: BUG-001_home_two-column-overflow.png

## Capture environment

- Browser: Google Chrome 140 on Windows 11
- Viewport: 1280x960 at 100% zoom
- Tools: Chrome DevTools for measuring spacing, colours and computed styles

## Evidence index: top bugs

| Bug ID | Module | Summary | Severity |
|---|---|---|---|
| BUG-045 | Prepare | Signature field cannot be moved, resized or deleted | P1 |
| BUG-047 | Global | Unexpected /grade.js script in page shell | P1 |
| BUG-048 | Global | Tech stack differs from original | P1 |
| BUG-001 | Home | Two-column row overflows container at 1280px | P2 |
| BUG-004 | Home | Start an agreement button disabled | P2 |

## Full evidence links

Links for all 60 bugs, including clone versus original comparisons, are listed in the Evidence column of the bug tracker spreadsheet. All links are set to anyone with the link can view.

## Note

Login credentials for the client's clone app are intentionally not shown in any screenshot or recording in this repository
