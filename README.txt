Basketballverse
v0.89.2 · Next Season Hard Fix

OFFICIAL NAME
The game is now Basketballverse.
Internal browser-storage keys remain unchanged so existing saves remain compatible.

NEXT SEASON HARD FIX
The accumulated legacy beginNextSeason wrapper chain is no longer used by the final
offseason button.

Start Next Season now uses one direct transition that:
- verifies only the real opening-night roster minimum/maximum
- automatically gives drafted rookies their rookie contracts
- saves outgoing season/draft/history/newspaper data
- advances the year
- processes expansion/realignment
- initializes the new regular season
- uses a guaranteed fallback initializer if a secondary system fails
- resets GM yearly workflow/objectives
- saves, renders, and opens the Season tab
- attempts to show the opening newspaper, but newspaper failure cannot block the season

Any secondary-system error is recorded as a warning instead of trapping the user in
the offseason.

Upload index.html and README.txt to the GitHub Pages repository root.
