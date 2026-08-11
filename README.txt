Basketball Universe League
v0.88.6 · Roster Limits Fix

BUG
The screenshot showed:
ReferenceError: Can't find variable: rosterLimits

CAUSE
Older GM/offseason systems still call rosterLimits(), while the current core
game uses rosterLimitForYear() and offseasonRosterLimitForYear().

FIX
- Restored a rosterLimits() compatibility helper.
- Maps activeMax / regularLimit to rosterLimitForYear().
- Maps offseasonMax / offseasonLimit to offseasonRosterLimitForYear().
- Keeps older GM checklist/readiness code compatible with the newer roster-limit engine.
- Clears stale rosterLimits error cards after load.

This is a targeted compatibility fix; it does not replace the working simulation engine.

Upload index.html and README.txt to the GitHub Pages repository root.
