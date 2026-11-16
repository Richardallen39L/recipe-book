Recipe Book v3.0.0 (web, Google Drive)
======================================
Same app as Recipe Book 2.7 on Windows, but it runs in the browser (PC and tablet) and keeps
its data in Google Drive, like Cheese Book.

Changes from 2.7
- Data: Drive folder "Recipe Book Data" (created by the app; sub-folders recipes, notes, reference, files).
- No Cheese tab, no pate making log (old log entries become notes), no Quit/data-folder/backup/smart-import.
- Notes are plain notes. Method is just the Method text.
- Top line: tabs ... [New recipe] [Search] ... Salt report, Fat, Ranges, Reference, Settings.
- Sync status badge bottom-right (tap for Drive status). Settings has Sync now / Export / Import.

Install (same as Cheese Book)
1. Create a GitHub repo (e.g. recipe-book), upload everything in this folder, enable Pages.
2. Open https://richardallen39l.github.io/recipe-book/ (the same Google sign-in client as Cheese Book is used;
   its authorised origin is the whole github.io site, so nothing to add).
3. First run: sign in, then Welcome screen -> choose the export file from 2.7
   (2.7 Settings -> Export everything (.json)). Cheese recipes in it are skipped.
4. On the tablet: open the same address, sign in, "Add to Home screen".

"Open file" links (recipes' Source file, notes' Linked file)
They are looked up by file name in your Drive (so your Recipe Book/recipes folder works).
This needs the extra read-only permission https://www.googleapis.com/auth/drive.readonly:
Google Cloud console -> APIs & Services -> OAuth consent screen -> Data access -> Add scope.
Then in the app: Settings -> Allow access to my Drive files. Without it everything else still works.

Import from file (.pdf/.docx/.txt) reads the file in the browser; the pdf/docx readers load from cdnjs when first used.
