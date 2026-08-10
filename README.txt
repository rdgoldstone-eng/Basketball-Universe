Basketball Universe League
v0.83.3 · Re-Signings Position Fix

BUG FOUND
The free-agency screenshot exposed a real function-name collision.

An older AI roster function used positionGroup() to return:
- Guard
- Wing
- Big

A later coaching/depth-chart system accidentally created another global function
with the SAME name that returned:
- PG
- SG
- SF
- PF
- C

The second function overwrote the first one. Re-signings then tried to do:
groups["PG"].push(...)
but the groups object only had Guard/Wing/Big, causing:
undefined is not an object (evaluating 'groups[positionGroup(p.pos)].push')

FIX
- Renamed the depth-chart helper so it no longer overwrites the AI roster helper.
- Added defensive position grouping so an unknown position can never crash re-signings/free agency.
- Added weakestGroup compatibility used by later AI systems.
- Existing saves already sitting at Free Agency clear the stale Re-signings error on load.
- The main offseason button is restored to "Complete Free Agency → Roster Cuts".

TEST RESULT NOTED
The user's Viewer test passed:
regular-season simulation intervals, trade deadline, All-Star break, end regular
season, playoff day, watch next game, finish series, and finish round.
This build fixes the remaining offseason error shown in that test.

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root.
