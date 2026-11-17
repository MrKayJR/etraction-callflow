# Etraction CallFlow

Daily call management and light CRM for Etraction Tyres. A single-file web app (`index.html`), no build step.

## Run
Open `index.html` in a browser, or serve the folder (for example `python3 -m http.server`).

## Use
1. Settings > Import workbook and choose your call list `.xlsx`. It is read in the browser and never uploaded.
2. Work from Daily Call Planner. Every call needs a comment.
3. Settings > Download backup (JSON) regularly. Data is stored in the browser's localStorage.

## Data safety
The repository contains no customer data. Never commit the Excel workbook or JSON backups (see `.gitignore`).

## Maintain
Everything lives in `index.html`: schedule defaults are in `DEF`, the scheduling logic in `pools()` and `plan()`, and the workbook import in `imp()`.
