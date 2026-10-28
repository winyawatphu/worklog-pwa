# WorkLog Monthly — Two Shifts & Workplaces

This version supports two separate shift sets per day. Each shift can have its own shift code, workplace, start/end time, break, OT and note. Monthly totals, history, calendar, and CSV export include both shifts.

## Add/edit workplace OT rates
Open the app and use **ตั้งค่า OT → สถานที่ทำงานและอัตรา OT**. Existing defaults are Somdej17 = 100 THB/hour and SPM = 200 THB/hour. Add another workplace by entering its name and OT rate. A workplace already used in a saved shift cannot be deleted until no saved shifts use it.

## Deploy to GitHub Pages
1. Export a JSON backup from your current WorkLog first.
2. Unzip this archive.
3. Upload all files inside this folder to the root of your existing `worklog-pwa` repository, replacing files with the same names. Keep `index.html`, `service-worker.js`, and `manifest.webmanifest` at repository root and include the `icons` folder.
4. Commit changes and wait for GitHub Pages deployment to succeed.
5. Open the website and force-refresh (Command + Shift + R on Mac).

Existing saved data is kept in browser local storage. This update preserves the existing first shift fields and adds an optional `shift2` object per date. Export JSON before updating.
