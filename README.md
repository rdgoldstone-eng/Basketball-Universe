# Basketballverse v0.96.32
## 1947 Playoff Button / Entry Fix

Built directly from v0.96.31.

Root cause found:
v0.96.31 correctly added the historical 1947 BAA bracket, but the Season screen's
OPEN PLAYOFFS button had already captured a reference to the older runPostseason()
function before the v0.96.31 override was installed. Replacing window.runPostseason
later therefore did not replace that button's saved click handler.

This build:
- uses the actual season.year to identify the inaugural 1946-47 season
- replaces the global runPostseason entry point
- explicitly rewires OPEN PLAYOFFS
- explicitly rewires BEGIN PLAYOFFS
- uses click delegation so newly re-rendered buttons are also caught
- creates the accurate six-team 1947 BAA bracket
- switches immediately to the Playoffs tab
- preserves the v0.96.31 historical playoff format and all prior game systems

A clean save is NOT required for this fix.
