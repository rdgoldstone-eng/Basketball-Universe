Basketball Universe
v0.82.12 · Newspaper Opening Screen Fix

CHANGE OF APPROACH
The existing Season Chronicle card has proven unreliable as an automatic transition.
This build no longer depends on that hidden card to make the newspaper appear.

NEW FLOW
- Start Next Season completes the season transition.
- The game moves to Season.
- A dedicated full-screen newspaper is placed directly over the Season page.
- The paper is generated from the season that just ended.
- Continue to Game 1 closes the paper.
- The normal Season page is immediately underneath, still at Game 1.
- Continue does NOT simulate a game.

SAVE REPAIR
If an existing save is already at Game 1 and the opening paper has not been acknowledged,
the newspaper is shown automatically after load.

EXPECTED
Offseason → Start Next Season → Newspaper → Continue to Game 1 → Season

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root.
