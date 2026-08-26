# Basketballverse v0.97.01
## Recovery Baseline

The first v0.97.00 cleanup attempt removed runtime layers too aggressively and
could prevent the game from loading.

v0.97.01 intentionally returns to the exact confirmed-working v0.96.39 runtime.
No Draft Room, playoff, save, portrait, logo, historical, ABA, merger, or
offseason logic has been removed or rewritten in this build.

This gives us a safe baseline before the cleanup/refactor is attempted again in
smaller, testable pieces.

Confirmed behavior carried forward from v0.96.39:
- game loads
- Viewer Draft Room displays the loaded historical prospect list
- permanent Sim This Pick / Sim Rest of Draft controls
- existing save compatibility
