Recipe Book v3.11.1 (web, Google Drive)
Upload the files in this folder to your GitHub Pages repo (replace the old ones).

New in 3.11.1
- Settings -> Drive & data -> "Show what the app sees in Recipe Book Data": lists the Recipe Book Data / files folders and every file the app can see, with a search box and a Copy list button. Use it to find out why a linked file is not found.
- Check source files shows the app version, and for a file that is not found it lists the closest names in Recipe Book Data and any error from the folder search.

In 3.11.0
- Open file and Check source files now look first in Drive -> Recipe Book Data -> files and all its sub-folders for a linked file given by name or path. Names are compared ignoring case, punctuation and the file extension, so "1001 Sausage Recipes - Index.xlsx" finds "10-01 Sausage Recipes - Index.xlsx"; when several files match, the one whose folder matches the folder in the stored path wins. If nothing is found there, the whole Drive is searched as before.
- "Make N name-based links permanent" now also covers files linked from notes.

In 3.10.1
- Open file no longer trusts an old remembered link: it checks the remembered file still exists (not deleted or in the Trash) and otherwise searches Drive again, preferring the newest copy. This fixes links that stopped working after files were moved or re-uploaded.
- Check source files now also lists the files linked from the Notes tab.

In 3.10.0
- Ingredient flags: ingredients that are typical of ultra-processed food (cutter phosphate / Kutterhilfsmittel, flavour enhancers such as MSG and yeast extract, glucose syrup / maltodextrin / dextrose, carrageenan, xanthan and other texture additives, protein isolates, emulsifiers, colours and smoke flavour, preservatives, ready-made seasoning blends) get a flag next to the ingredient, in the recipe editor as you type, and an "Additives" line at the top of the recipe. Click it for the list with the share of the mix, why it is flagged and a workaround. Curing salt / nitrite is shown but not counted (safety ingredient, no substitute).
- Settings -> Ingredient flags: edit the words (any language), the notes, switch rows off or add your own.

In 3.9.0
- Check source files: "Found by name" is treated as fine (listed after the real problems); making it permanent by ID is optional. "Tick all with no source file in [tab]" lets you pick one tab (for example the Sausage tab) and give all its blank recipes the Sausage Calculator workbook as their source in one go.

In 3.8.0
- Check source files: a Tab column, tick boxes on recipes without a working source file, and "Use this file for the ticked recipes" - type a file name (for example Sausage_Calculator_v30.xlsm) and every ticked recipe gets that file as its source. For recipes that only exist in a workbook.

In 3.7.0
- Settings -> Check source files: lists every recipe as linked by ID, found by name, found in several places, not found, linked file gone/in the Trash, or no source file, with the Drive folder each file is in. Copy report puts the list on the clipboard. "Link N found files by ID" turns name-based sources into ID links (they then survive renaming or moving the file). Needs "Allow access to my Drive files" once.

In 3.6.0
- Every recipe now shows a Source file card, even when it has none ("No source file yet" with an Attach file button). Attach file copies the file into Drive (Recipe Book Data/files) and links it by ID, so it still opens if the file is renamed or moved. The editor has Attach file and Clear buttons beside the Source file box.

In 3.5.0
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
