# Basketballverse v0.96.34
## Core 1947 Playoff Initialization Fix

This build was made after inspecting the actual uploaded Viewer save.

Verified save state:
- startYear: 1946
- currentYear: 1946
- season.year: 1946
- role: Viewer
- phase: Regular Season Complete
- 11 teams: 6 East / 5 West
- every team completed 82 games
- playoffState is absent

The save is healthy. The failure is in the game code.

Previous fixes were appended overrides. v0.96.34 changes the original CORE
initPostseasonExperience() function itself. When season.year is 1946 it creates
the historical six-team 1947 BAA bracket before the generic later-era
6-teams-per-conference logic can run.

The original runPostseason() function is also changed in place so it:
1. initializes the postseason,
2. verifies playoffState exists,
3. sets phase to Playoffs,
4. saves immediately,
5. opens the Playoffs screen.

No new save is required.
