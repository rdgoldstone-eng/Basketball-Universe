# Basketballverse — v0.97.52

## Current Build

**v0.97.52 · Safe Historical Draft Repair**

## Changes in v0.97.52

- Rebuilt directly from the last known-good v0.97.50 startup code.
- Removes the v0.97.51 startup-time state rebuild and forced full-page rerender that could prevent the webapp from loading.
- Loads the correct historical class only when the game requests the upcoming draft.
- Repairs the 1956–1977 class handoff, including the real 1976 class during a 1975 season.
- Gives historical prospects their matching lowercase underscore portrait keys.
- Preserves existing saves and does not rewrite completed draft results.
- Preserves the v0.97.50 Watch Game exit fix and earlier simulation visuals.

## Installation

Replace the repository-root `index.html` and `README.md` with these files. Keep all existing `logos/`, `portraits/`, and other asset folders in place. Existing saved universes remain compatible.
