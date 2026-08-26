# Basketballverse v0.96.37
## Draft Room DOM Rescue

The v0.96.36 screenshot proved that an older/later Draft Room wrapper was still
redrawing the visible screen after the repaired renderer. The save itself already
contains the 1947 draft order and 30 prospects.

v0.96.37 therefore fixes the visible DOM directly while the Draft stage is active:
- forces Sim This Pick and Sim Rest of Draft controls into the on-clock panel
- forces the loaded draftRoom.available prospects into the visible board
- refreshes the board after other legacy render wrappers run
- uses the existing v0.82.4 hard draft-pick engine for selections
- exposes Continue Offseason when the draft completes

No new save is required.
