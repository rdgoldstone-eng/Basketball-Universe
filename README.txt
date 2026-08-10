Basketball Universe
v0.82.15 · Permanent Archive Store

WHY THIS IS DIFFERENT
The prior fixes still stored Newspaper and Draft History only inside the giant main universe object.
Both features disappearing together strongly suggests the archive data is being lost during the main
save/transition lifecycle.

This build gives history its own small permanent storage area.

NEW PERMANENT ARCHIVE
- Newspaper editions are stored separately by universe + season.
- Draft histories are stored separately by universe + draft year.
- History screens merge those records back into the current universe whenever they open.
- The main season save and the history archive can no longer overwrite each other.
- A season transition cannot erase Draft History when Draft Room is reset.
- A later season cannot erase the previous newspaper.

EXISTING SAVE REPAIR
- Completed season history is used to rebuild missing newspaper editions.
- Existing draft history and player draft stamps are used to rebuild missing drafts where possible.
- Recovered records are then written into the permanent archive.

IMPORTANT
This is intentionally a storage-layer fix, not another timing/render patch.

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root.
