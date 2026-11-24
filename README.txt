Recipe Book v3.23.0 (web, Google Drive)
Upload the files in this folder to your GitHub Pages repo (replace the old ones).

New in 3.23.0
- Unrecognised tab: the recipe names are now links. Click one to open that recipe in the editor (you can add the ingredient to the norms with the + button there, or rename the line). Save, or Cancel, returns you to the Unrecognised list, which has refreshed. Opening a recipe any other way, or switching tab, forgets the return. A long list of recipes is cut to five names with a "+n more" link that shows the rest.

In 3.22.0
- Settings has a new tab, Unrecognised, holding the Ingredients not in the list card (moved from Salt & Fat). The tab name shows how many ingredients are unrecognised, for example Unrecognised (4), and the count drops as you add them with the + button. This tab needs no Save settings button because each + saves straight away.

In 3.21.0
- Ingredients not in the list: a new card at the top of the page that holds the Ingredient norms (Settings), listing every ingredient in all your recipes that the Ingredient norms do not recognise, with how many recipes use it and a note where the name is genuinely ambiguous (fennel: seed or bulb; ginger: fresh or ground; cloves; garam masala; vanilla; horseradish; soy protein; plain pepper). Click + to add one with your own figures; the list refreshes. The add dialog shows the same note.

In 3.20.0
- Check source files: a linked file that is in the Bin or has gone now gets the same drop-down as the other problem items. It offers any live file in Drive with the same name, and Link this one switches the recipe or note to it.
- Staying signed in to Google Drive (tablet): Google only issues sign-ins that last about an hour, and a tablet browser blocks the small sign-in window unless you have just tapped. The app now (1) remembers which Google account you used, so no account chooser is shown, (2) renews the sign-in on your first tap once it has run out or is within 10 minutes of running out, which is when the browser allows the window, and (3) records each sign-in in the Drive status window (tap the sync indicator), with whether the sign-in and account are kept on this device. The app never uses GitHub: it is only hosted there.

In 3.19.0
- Spices and herbs added to the built-in Ingredient norms (list version 5): black and white pepper, paprika, cumin, cayenne, curry powder, turmeric, cinnamon, cardamom, nutmeg, mace, allspice, fennel seed, caraway, juniper, star anise, saffron, fenugreek, ground and fresh ginger, thyme, marjoram, oregano, sage, rosemary, bay leaf, basil, mint, dill, tarragon, chives, plus dextrose, brandy, barley, morel, casing, starter culture and bactoferm. Dried and fresh herbs have separate rows ("Dried thyme" uses dried figures, plain "Thyme" fresh ones). A list you have already saved keeps everything it has, including your own edits and rows, and simply gains any of these it does not already contain; nothing is overwritten. Still deliberately unrecognised because they are ambiguous: fennel (seed or bulb), ginger, cloves, garam masala, vanilla, horseradish. Use the + button to add them with your own figures.
- Lard stays typed as meat on the Sausage tab.

In 3.18.0
- Moving ingredients in the editor: clicking a line's up or down arrow now selects that line (it is highlighted) and shows a move bar that stays fixed at the top of the ingredient list: Moving <name> (line n of m), with Up, Down and Done buttons. Click Up or Down on the bar as many times as you like without moving the pointer; the line carries on moving and stays in view. Alt+Up / Alt+Down on the keyboard do the same. Done (or deleting the line) clears the selection.

In 3.17.0
- Unrecognised ingredients are flagged. An ingredient whose name is not found in Settings -> Ingredient norms (no salt, fat or each-weight row matches, and you have not typed your own salt or fat for the line) is shown with its name in quotes and a small + button in the recipe, and with a dashed name box, a + button and a note under the table in the editor and the import review. Click the + to add it to the Ingredient norms (words in the name, salt %, fat %, optional weight of one item); the flag then disappears everywhere. Until then its salt and fat count as 0. The flag does not print.
- Meat words: Settings -> Ingredient norms has a new Meat words box. On the Sausage & bacon tab an imported ingredient is typed as meat when its name contains a built-in meat word or one of the words you add there. The built-in list now also has sausage, kielbasa, chorizo, salami, pancetta, lardons and prosciutto.

In 3.16.0
- Back and forward buttons (arrows at the top left of the header): step back and forward through the recipes and notes you have looked at, across tabs too. Also Alt+Left / Alt+Right on the keyboard and the back / forward buttons on a mouse. From Settings, Search and so on, Back returns to the last recipe. If you have unsaved edits you are asked before leaving.
- Import fixes (found with the Polish Rejbak recipe, which lost all its meat lines): an ingredient line with no amount, such as "Salt and plenty of freshly ground black pepper", no longer ends the ingredient list while more ingredients follow; sub-headings such as "Potato mixture" and "To grease and serve" are read as groups; amounts like "750g-1kg" are read as a range (the midpoint is used, as for other ranges); PDF page headers such as "Polish Rejbak - 1" no longer become the recipe name; and long one-line method paragraphs are split into separate steps.

In 3.15.0
- Pork substitute: on a Sausage & bacon recipe with a pork shoulder or belly line, Make this recipe has a "Pork substitute (loin + back fat)" tickbox. Ticked, the shoulder / belly lines show 0 and the pork loin line is added (or increased, if the recipe already has a pork loin / lean pork line) and the back fat line is added or increased, keeping the same total weight and the same fat (loin and back fat fat% come from Settings -> Ingredient norms). The loin line becomes the "By ingredient" reference, so type the weight of loin you have and everything else scales to it. Salt, fat and % of meat all follow the swapped amounts. Ticking or un-ticking keeps the batch at the same multiple of the recipe. The saved recipe is never changed unless you press Use as the recipe (it then replaces the shoulder / belly lines with the loin and back fat shown).
- This replaces the "Using loin and back fat instead" card and the "Total loin" scaling choice from 3.14.0.

In 3.14.0
- Text size: Settings -> Organisation -> Text size (Normal, Large, Larger, Largest). It scales the text everywhere in the app and is kept per device, so the tablet and the PC can differ. The default is now Large (a little bigger than before). Printing always uses the normal size.
- "Using loin and back fat instead": the card now always ends with a Total loin to buy line (with the total back fat to add), and "Total loin (if using loin and back fat instead)" is a new choice in Make this recipe -> By ingredient. Type the weight of loin you have and the whole recipe scales to use exactly that much loin.

In 3.13.0
- Filter dropdown: under the filter box the list now holds All, Favourites, the salt option and every category of the current tab (with the number of recipes in each). On the Notes tab it holds All and the note kinds.
- The filter text and dropdown are cleared when you swap tabs.
- Catalogue: the app keeps two spreadsheet-style lists in Recipe Book Data. catalogue.csv has one row per recipe and note (tab, category, favourite, source file ID, file name, link) and is updated a few seconds after each save. originals.csv lists every file in the files folder with its folder and which recipes use it (files nothing uses show a count of 0); it is updated by Check source files and by Settings -> Drive & data -> Update catalogue now.
- Check source files is now quiet and quick: files linked by ID are confirmed from one listing of the files folder instead of one Drive call each, and the report shows only what needs a decision. One button links every found-by-name file by ID; recipes found in several places or with a possible match get a drop-down to choose the file and a Link this one button. Recipes with no source file are tucked under their own heading, and the full list is under Show all.

In 3.12.0
- Linked files are now also matched approximately inside Recipe Book Data / files: if no file has the same name (ignoring case, punctuation and extension), a single file whose name shares most of its words (for example an extra "v2" or "copy") is used. Open file uses it; Check source files lists it as "Possible match (please check)" with the file it found, and "Link N possible matches by ID" fixes them after you have looked at the list.

In 3.11.1
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
