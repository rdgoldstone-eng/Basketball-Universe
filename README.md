# Basketballverse — v0.97.50

## Current Build

**v0.97.50 · Watch Game Exit Fix**

## Changes in v0.97.50

- Fixes the completed Watch Game screen losing its Continue Playoffs button during the second playoff render pass.
- Keeps the current Watch Game action in place while the live scoreboard refreshes.
- Guarantees a Continue Playoffs button when a watched game reaches FINAL.
- Continue Playoffs closes the watched game, returns to the postseason matchup view, and restores the normal playoff simulation controls.
- Preserves the v0.97.49 playoff result pause and Next Game flow.

## Installation

Replace the repository-root `index.html` and `README.md` with these files. Keep all existing `logos/`, `portraits/`, and other asset folders in place. Existing saved universes remain compatible.
