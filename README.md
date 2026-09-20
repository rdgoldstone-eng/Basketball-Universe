# Basketballverse — v0.97.66

## Current Build

**v0.97.66 · Founding Decision Repair**

## Changes in v0.97.66

- Fixes the screen recovery warning `undefined is not an object (evaluating 'd.choices.map')` after starting the 1947–48 season. Founding franchise decisions were saved with an `options` list, but the general Decision screen assumed every pending decision had `choices`.
- Displays the existing founding franchise choices from saved games and gives newly created decisions both compatible lists. Commissioner choices still apply to the franchise; saved decisions are not removed or resolved automatically.
- Retains the v0.97.65 fix that correctly shows the active 1947–48 regular season and clears the old playoffs.
- Updates the page banner, watermark, and build metadata to v0.97.66.

## Installation

Replace the repository-root `index.html` and `README.md` with the files in this folder. Keep your existing `portraits/`, `logos/`, and other asset folders. Existing browser saves stay in place.
