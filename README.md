# Basketballverse — v0.97.64

## Current Build

**v0.97.64 · Saved Season Display Repair**

## Changes in v0.97.64

- Verified against an exported Commissioner save: the save is in the 1947–48 regular season with zero games played, no active offseason, and the new teams already loaded. The 1946–47 displays were stale.
- Refreshes Season after a save loads, after navigation, and after the year transition. Its current-year header, scoreboard, simulation buttons and standings can no longer remain on the prior season's completed view.
- Clears the prior year's playoff title, Finals matchup, game log, watch-game panel, and controls when the current year has not yet started its playoffs.
- Preserves the existing league history, saved results, and offseason actions already completed. Keeps prior expansion, decision and draft fixes.

## Installation

Replace the repository-root `index.html` and `README.md` with these files. Keep your existing `portraits/`, `logos/`, and other asset folders. Your save stays in the browser; opening it should show 1947–48 at the start of the regular season.
