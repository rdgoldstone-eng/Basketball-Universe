# Basketballverse v0.91.49 — GM Playoff Objective Fix

## Fix in this build
- Fixes GM playoff objectives incorrectly showing as incomplete after a successful playoff run or championship.
- The Objectives system now reads the canonical `state.season.playoffState` used by the actual postseason.
- Playoff achievement is hierarchical:
  - 1 = made playoffs
  - 2 = reached semifinals / second round
  - 3 = reached conference finals
  - 4 = reached NBA Finals
  - 5 = won NBA championship
- Winning a championship automatically satisfies lower-level playoff goals such as **Make a playoff run**.
- First-round byes are recognized correctly in historical playoff formats.
- Works with an active postseason and with a completed championship season.
- Retains the v0.91.48 historical first-round format correction.
- In-game version banner updated to v0.91.49.

## Installation
Upload/replace the files from this ZIP in the same GitHub location used for Basketballverse.

## Save compatibility
Compatible with existing saves. The objective is recalculated from the postseason data already stored in the save, so a championship already won in the current season should be credited when the Objectives page refreshes.

## Test
1. Load a save in which your controlled team has reached at least the second round.
2. Open **Objectives**.
3. **Make a playoff run** should show complete.
4. If your team won the NBA championship, every playoff-achievement objective below championship level should also be complete.
