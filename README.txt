Basketball Universe
v0.82.11 · Newspaper Generation Fix

WHAT WAS ACTUALLY WRONG
v0.82.10 fixed WHEN the newspaper was supposed to appear, but it still assumed
a completed newspaper object already existed after Start Next Season.

In some saves, the season transition changed/cleared the data before the
newspaper was marked pending. Result: correct timing logic, but no paper existed
to display.

FIX
- The completed-season newspaper is now captured/generated BEFORE the year changes.
- That snapshot is carried into the new season and marked pending immediately.
- Start Next Season then opens the Season page and forces the newspaper card visible.
- The newspaper has its own Continue button.
- Continue closes the paper and leaves the user at Game 1.
- Added a fallback newspaper renderer if an older save's newspaper object is incomplete.
- Existing saves already at Game 1 can reconstruct the paper from the previous season's history.

EXPECTED FLOW
Start Next Season
→ previous season newspaper appears immediately
→ Continue
→ Game 1

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root.
