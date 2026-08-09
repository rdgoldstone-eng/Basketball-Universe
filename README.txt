Basketball Universe
v0.82.3 · Draft Simulation Fix

BLOCKER FIX
- Fixed "Sim This Pick" so an AI evaluation error cannot silently freeze the draft.
- Added a safe fallback prospect selection if normal AI draft-choice logic fails.
- Rebuilt "Sim Rest of Draft" as a true batch simulation.
- The old version re-rendered and saved the entire universe after every single pick; on phones this could take so long that the button appeared to do nothing.
- Batch simulation now performs all remaining picks first, then renders/saves once.
- GM/Owner "Sim to My Pick" still stops when the user's franchise is on the clock.
- Viewer/Commissioner "Sim Rest of Draft" runs all remaining selections.
- Added a guard so a stuck pick cannot create an endless loop.
- Malformed draft names are repaired before and after simulation.

TEST
At the Draft stage:
1. Open Draft Room.
2. Tap Sim This Pick. The pick number should advance immediately.
3. Tap Sim Rest of Draft in Viewer mode. The draft should finish and display the results.
4. Continue Offseason should then become available.

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root, replacing the previous files.
