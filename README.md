# HisabSaathi MVP

A free, beginner-friendly prototype for personal expenses and shopkeeper income/expense records.

## Included
- Personal and Shopkeeper modes
- Manual Cash, UPI, Bank, Card and Other entries
- Income and expense totals by selected month
- Search and filters
- CSV export
- Local browser storage
- PWA manifest and service worker for installation/offline caching when hosted over HTTPS

## Important limitations
- This prototype does NOT connect to a bank, UPI app, SMS inbox or payment provider.
- UPI transactions must be entered manually.
- Data stays in this browser/device. It does not sync between devices and may be lost if browser data is cleared. Export CSV backups regularly.
- Not production-ready for sensitive financial records; add authentication, secure backup, privacy policy and security review before a public commercial launch.

## Run locally
1. Extract this folder.
2. Open `index.html` in a browser for basic testing.
3. For PWA/offline installation testing, host the files over HTTPS (GitHub Pages is one free option).

## Publish on GitHub Pages (free)
1. Create a GitHub repository named `hisabsaathi`.
2. Upload `index.html`, `manifest.json`, `sw.js`, and `icon.svg` to the repository root.
3. In repository Settings → Pages, select deploy from the `main` branch and `/ (root)`.
4. Open the published HTTPS URL on Android Chrome.
5. Chrome menu → Add to Home screen / Install app (wording varies).
6. Test adding, editing/deleting, filtering and exporting entries on the phone.

## Suggested test cases
- Add ₹250 expense by UPI and ₹100 expense by cash; verify spent total is ₹350.
- Add ₹1,000 income; verify received total is ₹1,000 and net difference is ₹650.
- Switch Personal/Shopkeeper: records should remain separated.
- Change month: only selected-month records should count.
- Export CSV and open it in a spreadsheet app.
- Turn on airplane mode after first online visit and verify cached app opens.
