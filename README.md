# Basketballverse — v0.97.63

## Current Build

**v0.97.63 · Season Screen Recovery**

## Changes in v0.97.63

- Refreshes the Season and Playoffs screens after starting a new season, clearing the prior year's completed scoreboard and playoff controls.
- Repairs a saved universe whose year advanced while its completed season object was left behind. The recovery runs when the game loads or when Season, Playoffs, or Offseason is opened.
- Preserves completed history and earlier saves; it only initializes the new season when the saved year is ahead of the season year and no unfinished prior offseason remains.
- Retains the Commissioner expansion and seasonal review fixes.

## Installation

Replace the repository-root `index.html` and `README.md` with the two files in this ZIP. Keep your existing `portraits/`, `logos/`, and other asset folders. Saved universes remain in the browser.

For the currently affected save, open the Season tab once after updating. The screen should show the new regular season and reset standings rather than the completed 1946–47 season.
