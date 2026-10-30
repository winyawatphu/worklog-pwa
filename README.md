WorkLog PWA — Two shifts in one row + dynamic workplace OT summary

What's changed:
- Each calendar date is displayed as ONE row.
- Shift 1 and Shift 2 are side-by-side in grouped columns, similar to the provided spreadsheet.
- Existing shift 1 and shift 2 data structure is retained; no migration or clearing of browser storage is required.
- Workplace summary is dynamic and includes every configured workplace, including Lotus.
- CSV export includes both shifts, workplace, OT rate, OT hours, OT income, new-shift field and notes.
- Service worker cache name is bumped to v6.

Deploy:
1. Back up JSON from the current app.
2. Extract this ZIP.
3. Upload the CONTENTS of WorkLog_PWA_Two_Shifts to the ROOT of the existing GitHub Pages repository, replacing same-named files. Keep index.html at repository root.
4. Commit and wait for GitHub Pages deployment to finish.
5. Open the site and hard refresh (Cmd+Shift+R on Mac).

Data remains in each browser's local storage. Do not clear site data during update.
