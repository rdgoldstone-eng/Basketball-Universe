Basketballverse
v0.91.7 · Play Button Hard Fix

WHY THE PREVIOUS FIX WASN'T ENOUGH
The saved-game list was still built from HTML strings with click behavior layered on afterward.
On mobile Safari, that path was still not reliably triggering the saved-game loader.

HARD FIX
- Saved Universe rows are now built as real DOM elements.
- The Play button gets a direct addEventListener() when the row is created.
- Tapping Play immediately changes the button to "Opening…" so there is visible feedback.
- The game view is revealed before the rest of the save rendering runs.
- The old playSavedUniverse() public function now routes through the same hard-fix loader.
- Rename and Delete buttons are also attached with direct listeners.

Existing saves are preserved.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
