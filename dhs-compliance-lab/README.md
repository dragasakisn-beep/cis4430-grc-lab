# CIS 4430 — GOV Personnel Information Exposure Lab, v1.5

GitHub Pages-ready, client-only GRC investigation workbench for Keiser University.

## What changed in v1.5

- Fixed and retested PowerPoint creation: output is generated as a Blob and offered as an `.pptx` download. The presentation archive passed ZIP validation in a local Node test.
- Replaced horizontally scrolling data-entry tables with labeled record cards for sources, applicability, IAM controls, evidence, risks, and POA&M. Inputs, selects, and date fields save on each edit.
- Made the three main actions contiguous: Submission Check, Print/Save PDF, and Export PowerPoint.
- Redesigned responsive academic banner and navigation with a vector banner background.
- Clarified **only required deliverable**: the final completed printed report (or PDF equivalent if the instructor accepts it). PowerPoint and workspace backup are optional.
- Preserved project autosave, backup, import, grading rubric, and all 10 investigation sections.

## Deploy without overwriting the existing repository homepage

1. Open `dragasakisn-beep/cis4430-grc-lab` on GitHub.
2. Navigate to the `dhs-compliance-lab` directory.
3. Replace these files with the files from this directory: `index.html`, `app.js`, `styles.css`, `academic-banner.svg`, and `vendor/pptxgen.min.js` (if absent). Also keep `vendor/LICENSE-pptxgenjs.txt`.
4. Commit the modifications on the `main` branch.
5. Open `https://dragasakisn-beep.github.io/cis4430-grc-lab/dhs-compliance-lab/`, perform a hard refresh, and test input and downloads in Chrome or Edge.

The legacy `/dhs-compliance-lab/` folder name is retained so existing course links remain valid. The visible case title is GOV Personnel Information Exposure.

## QA performed

- Node syntax check: passed.
- Functional unit check (text entry, selection, persistence callback, print HTML generation, validator): passed.
- Node PowerPoint generation test: passed; produced valid `.pptx` ZIP structure.
- Browser end-to-end testing: **not completed** because the test environment blocked browser navigation. On-site test is required, especially on Safari/in-app browsers, where automatic file downloads may be restricted.

## Privacy and data integrity

All entries are stored in the student's browser profile. No central server, instructor collection, login, or automatic grade submission. Do not enter live government records, credentials, or protected information.

The reported DHS information exposure provides an attributed research starting point. The FSSC scenario and its records remain fictional; the identity system intrusion claim is unverified.
