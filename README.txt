Recipe Book v3.5.0 (web, Google Drive)
Upload the files in this folder to your GitHub Pages repo (replace the old ones).

New in 3.5.0
- Ingredient norms: fat % for pork loin 17.4, pork shoulder 24.3, pork belly 26.8 and back fat 100 (also "belly pork", "backfat", "fat back"). Settings you saved earlier are kept; only these rows are updated.
- A recipe with pork shoulder or belly now shows a card "Using loin and back fat instead": the loin and back fat weights that give the same total weight and the same fat as the cut in the recipe. It follows the scaling.

In 3.4.0
- The detailed Salt analysis, Salt & cure check and Fat analysis no longer sit under the ingredients. Click the Salt % or Fat % figure at the top of a recipe to open the detail in a pop-up (Esc or Close to dismiss).
- Import from file now reads recipes made of several parts (a heading, its ingredients, then its method, repeated): each part's ingredients are grouped under the heading and its method goes into the Method under the same heading. French or other languages are kept as written. "Ou 100 g ..." lines become a note on the ingredient above.

In 3.3.0
- Duplicate now numbers itself if "(copy)" already exists: Name (copy), Name (copy 2), and so on, so saving no longer fails on a name clash.

In 3.2.0
- The ☰ button at the top left shows or hides the recipe list so the recipe gets the full width. The choice is remembered on each device.

In 3.1.2
- Quit button restored (top right). It waits for pending Drive saves, then closes the window.
- Fixed the install clash with Cheese Book: the app manifest now has its own unique id (recipe-book).

In 3.1.1
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
