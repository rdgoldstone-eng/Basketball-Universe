Basketballverse
v0.89.3 · Objectives & Decision Cleanup

FIXES FROM GM PLAYTEST

1. OBJECTIVES TAB
Season navigation now includes:
- Season
- Decisions
- Objectives
- Playoffs
- Offseason

GM Objectives shows:
- owner objectives
- live progress
- job security
- reputation

Other roles have an Objectives placeholder ready for their role-specific goal systems.

2. FREE AGENCY RECAP
Free Agency recap/summary is informational, not a decision.
- It no longer counts in Decisions.
- Existing recap items from older saves are auto-resolved.
- Recaps remain appropriate for News / Offseason review.

3. SAFE TRANSITION ERROR
The screenshot showed:
ReferenceError: Can't find variable: safeTransitionStep

Cause:
safeTransitionStep existed only inside beginNextSeason(), while regular-season
milestones also called it.

Fix:
A global compatibility safeTransitionStep() is now available for regular-season
trade-deadline and other milestone maintenance. A secondary subsystem error is
logged instead of stopping the game.

4. BASKETBALLVERSE BRAND
Visible header/title branding is forced to Basketballverse.
Old browser-storage keys remain unchanged so saves stay compatible.

Upload index.html and README.txt to the GitHub Pages repository root.
