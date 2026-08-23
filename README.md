# Basketballverse v0.91.94 — Compact Status Compatibility Fix

Fixes the runtime error:
`document.getElementById("decisionKpi").textContent ... null is not an object`

v0.91.93 removed Open Decisions visually by deleting its DOM element. Older game rendering code still uses `decisionKpi` internally, so deleting the element caused rendering to crash.

v0.91.94:
- keeps a hidden `decisionKpi` compatibility target in the DOM
- keeps Open Decisions invisible to the player
- preserves the compact Season / Role / Team status presentation
- preserves the Owner arena / relocation / rebrand systems from v0.91.93

Parser check included.


## v0.92.00 — Draft Clock + Compact Header Fix
- Built directly from the known-good v0.91.99 package.
- Role / Team / Season header is now one genuinely compact horizontal row.
- Open Decisions remains hidden but its legacy DOM target is preserved for compatibility.
- Draft controlled-team comparisons normalize team IDs to avoid false "not on the clock" results.
- No Owner systems from v0.91.99 were removed.
