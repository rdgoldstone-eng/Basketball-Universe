Basketball Universe
v0.82.8 · Draft Completion & Redirect Fix

WHAT THE SCREENSHOT REVEALED
The draft was actually finishing. The error was happening AFTER the selections were completed, during the old global post-draft render path. That is why leaving the Draft Room and coming back showed a completed draft.

FIXES
- A completed draft no longer calls the problem global render path.
- Sim Rest of Draft saves the completed basketball state first, then automatically returns to the Offseason screen.
- The offseason automatically advances from Draft to Re-signings.
- Sim This Pick also auto-returns to Re-signings if it makes the final selection.
- If a save already contains a completed draft but is stranded on the Draft Room, it repairs itself on load.
- A completed Draft Room now has a working "Continue to Re-signings" button.
- Added defensive initialization for news, draft history, transactions, draft results, free agents, and draft-room arrays.
- The misleading "Cannot read properties of undefined (reading 'push')" error after an otherwise completed draft should no longer block progression.
- Includes the Viewer Free Agency / Roster Cuts finish-flow fixes from v0.82.7.

TEST
Use the same 1977 save.
Tap Sim Rest of Draft.
Expected behavior:
1. Draft completes.
2. Game automatically switches to Offseason.
3. Re-signings is highlighted as the current task.
4. You do not need to manually leave the Draft Room.

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root.
