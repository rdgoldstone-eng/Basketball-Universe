Basketball Universe
v0.82.1 · Draft Room Launch Fix

BLOCKER FIX
- Fixed the Draft Room submenu button after the navigation redesign.
- Clicking Draft Room during the Draft stage now actually initializes and opens the draft.
- Fixed the Draft Room navigation selector to recognize the current sub-navigation system.
- Added a defensive repair for saves that reached the Draft stage with an empty or partially initialized Draft Room.
- Direct calls to the Draft Room now re-render the room instead of leaving the "Draft is opening..." screen stuck.
- Existing saves should remain usable; a draft at the Draft stage will rebuild itself if necessary.

STATUS
This is a blocker fix for v0.82. Do not start the dedicated GM playtest yet; first confirm the Draft Room opens and runs normally.

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root, replacing the previous files.
