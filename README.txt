Basketball Universe
v0.82.7 · Offseason Finish Flow

WHAT THIS FIXES
- The screenshot showed Free Agency as the current task while the main button still said "Retry Re-signings."
- The offseason action button is now forced to match the ACTUAL saved phase every time the screen renders.
- Viewer Free Agency now runs through a fast phone-friendly league pass rather than the heavier AI roster-planning path.
- Free Agency shows completed signings and how many players remain unsigned.
- Complete Free Agency now advances directly to Roster Cuts.
- Viewer Roster Cuts now run through a fast batch process and show each team's final roster count.
- Complete Roster Cuts advances to Next Season.
- Start Next Season now has its own direct Viewer path.
- Existing saves already sitting on Free Agency or Roster Cuts repair themselves on load.
- Includes the v0.82.6 draft-state repair as well.

TEST
Use the same save from the screenshot.
1. Free Agency should remain highlighted.
2. The large yellow button should now say "Complete Free Agency → Roster Cuts."
3. Tap it.
4. Roster Cuts should highlight.
5. Complete Roster Cuts → Next Season.
6. Start Next Season.

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root.
