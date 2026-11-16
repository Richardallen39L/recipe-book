Recipe Book v3.1.1 (web, Google Drive)
Upload the files in this folder to your GitHub Pages repo (replace the old ones).

New in 3.1.1
- The version number (e.g. v3.1.1) is shown in the app header and in the window title.
- The service worker now bypasses the browser cache so an installed copy picks up new versions at the next open.
- New maskable icon (icon-maskable-512.png) so Android does not crop the app icon.

In 3.1.0
- Click any column heading in a list to sort: 1st click A-Z (or low-high), 2nd Z-A, 3rd back to the original order.
  Works in the recipe amounts, salt and fat analysis, reports, salt ranges, Ingredient norms, Units and Conversions.
  (Tabs, Categories and the recipe editor are not sortable because their order is something you set.)
- Settings has sub-tabs: Organisation (Tabs, Categories), Salt & Fat (Targets, Norms), Measures (Units, Conversions),
  Drive & data. Save settings applies to Salt & Fat and Measures.

Setup, Drive and Open-file notes are unchanged from 3.0.0:
Open file needs the drive.readonly scope added under Google Cloud -> OAuth consent screen -> Data access.
