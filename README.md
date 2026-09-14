# Basketballverse — v0.97.51

## Current Build

**v0.97.51 · Historical Class & Portrait Repair**

## Changes in v0.97.51

- Repairs the 1956–1977 historical draft-class handoff in existing saved universes before the next draft begins.
- Prevents a saved fictional draft pool from replacing the real 1976 class during a 1975 season.
- Restores recognizable 1976 prospects including John Lucas, Scott May, Adrian Dantley, Robert Parish, Alex English, and Dennis Johnson.
- Routes roster, scouting, draft, award, newspaper, and career portraits through the same `portraits/first_last.webp` convention.
- Adds a fresh portrait cache key so recently uploaded WebP files are requested again instead of using stale missing-image results.
- Leaves already completed draft results untouched to protect existing save history.
- Preserves the v0.97.50 Watch Game exit repair and prior simulation visuals.

## Installation

Replace the repository-root `index.html` and `README.md` with these files. Keep all existing `logos/`, `portraits/`, and other asset folders in place. Existing saved universes remain compatible.
