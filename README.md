# Basketballverse — v0.97.37

## Current Build

**v0.97.37 · Minneapolis Lakers Logo Repair**

Basketballverse is a browser-based professional basketball universe simulator spanning the league's historical eras. Create or load a universe, choose a role, and let league history develop through simulation and alternate-history decisions.

## Changes in v0.97.37

- Corrected the Minneapolis Lakers historical logo filename to `minneapolis-lakers-1948.webp`.
- Corrected the team's BAA branding start year from 1947 to 1948.
- The game now requests `./logos/teams/minneapolis-lakers-1948.webp`, matching the existing repository asset.
- Added a compatibility repair for saved universes that cached the old `minneapolis-lakers-1947.webp` path.
- Repairs the team's current logo, early-era logo library slot, and Minneapolis identity-history record before rendering.
- Preserved the v0.97.36 browser-state playoff repair and historical 1947–48 BAA postseason loop.
- Synchronized `v0.97.37` on the main page and persistent watermark.

## Verification

- All 153 inline scripts compile successfully.
- A browser-style saved-state test with no `window.state` repaired every cached Minneapolis logo reference.
- The historical resolver returns `./logos/teams/minneapolis-lakers-1948.webp` throughout 1948–1959.

## Repository Structure

```text
Basketball-Universe/
├── index.html
├── README.md
├── logos/
└── portraits/
```

The ZIP contains only the two files that change with this build:

- `index.html`
- `README.md`

Keep the existing `logos/` and `portraits/` folders in the repository. Confirm that the logo remains at:

```text
logos/teams/minneapolis-lakers-1948.webp
```

## Updating the GitHub Repository

1. Extract the ZIP.
2. Upload `index.html` and `README.md` to the repository root.
3. Allow GitHub to replace the existing files with the same names.
4. Keep the existing `logos/` and `portraits/` directories unchanged.

## Save Compatibility

Existing saved universes remain compatible. When a 1948–1959 save is opened or rendered, v0.97.37 replaces the obsolete cached Minneapolis path and saves the corrected logo reference.
