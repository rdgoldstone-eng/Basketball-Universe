Basketballverse
v0.91.34 · Division Standings Fix

BUG
The v0.91.32 workaround hid the first cell of every standings row. On a division
header, that first cell was the entire division label, so the standings became worse.

FIX
- Standings remain clearly split by division.
- Division headers remain visible.
- Ranking numbers are removed completely.
- The table is now built natively as:
  Team · W · L · PCT
- No post-render hiding tricks are used.

Retains all systems from v0.91.33.
