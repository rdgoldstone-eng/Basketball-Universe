# Basketballverse v0.96.36
## Draft Room Renderer Fix

Built after inspecting the exact uploaded stuck save.

The save already contains:
- offseason.phase = Draft
- draftRoom.active = true
- draftRoom.year = 1947
- pickIndex = 0
- 22 draft slots
- 30 available historical prospects
- 0 results

So the draft data was never missing. The failure was presentation/control-side.

v0.96.36 adds a Viewer-specific Draft Room renderer that reads the existing
draftRoom.available array directly and displays it without depending on the
controlled-team/scouting presentation path. It also supplies working:
- Sim This Pick
- Sim Rest of Draft
- Continue Offseason after completion

No save repair or restart is required.
