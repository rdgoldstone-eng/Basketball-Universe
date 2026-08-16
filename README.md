# Basketballverse v0.91.48 — Historical Playoff Format Fix

## Fix in this build
- Corrects the NBA first-round series format by season:
  - through 1983-84: best-of-3
  - 1984-85 through 2002-03: best-of-5
  - 2003-04 onward: best-of-7
- Specifically fixes 1993-94 so the first round is best-of-5.
- Adds a save-game compatibility guard. If an older save has an active first-round series incorrectly stored as best-of-7, Basketballverse repairs the active, unfinished series when the postseason loads.
- Synchronizes the displayed league-rule value with the historical playoff format.
- Retains the GM Career Profile, free-agency economy changes, lottery stability fixes, and earlier features.
- Updates the in-game version banner to v0.91.48.

## Installation
Replace the previous `index.html` with this build's `index.html`, or upload the contents of this ZIP to the same GitHub location used for Basketballverse.

## Save compatibility
Designed to work with existing Basketballverse saves. The playoff-format repair applies to active unfinished first-round series; completed historical series are not rewritten.

## Test
For the 1993-94 season, open the playoffs and confirm each first-round series displays **Best of 5** and clinches at three wins.
