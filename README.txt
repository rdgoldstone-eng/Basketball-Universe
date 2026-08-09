Basketball Universe
v0.82.5 · Re-Signings Flow Fix

BLOCKER FIX
- Fixed Viewer mode getting stuck at Re-signings.
- Re-signings now use a fast phone-friendly batch process instead of the heavier AI roster-planning path.
- Players either re-sign or enter free agency in one pass.
- The Re-signings detail panel now shows how many players stayed and how many entered free agency.
- Existing saves already parked at Re-signings are repaired on load.
- Complete Re-signings now advances directly to Free Agency.
- GM mode still keeps its manual contract decisions; this Viewer repair does not automate a controlled GM roster.
- Added visible error output if Re-signings itself fails instead of leaving the screen stuck.

TEST
Load the same save at Re-signings.
You should immediately see a Re-signings summary.
Tap "Complete Re-signings → Free Agency".
The current highlighted offseason task should move to Free Agency.

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root, replacing the previous files.
