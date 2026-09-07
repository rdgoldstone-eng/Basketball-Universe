# Basketballverse — v0.97.31

## Current Build

**v0.97.31 · Stable Sim Re-signings**

Basketballverse is a browser-based professional basketball universe simulator spanning the league's historical eras. Create or load a universe, choose a role, and let league history develop through simulation and alternate-history decisions.

## Changes in v0.97.31

- Replaced the competing Viewer-mode Re-signings simulation controls with one stable inline button.
- Removed the duplicate floating Sim Re-signings control.
- Sim Re-signings now processes league re-signings exactly once.
- After simulation, the offseason advances exactly once from Re-signings to Free Agency.
- Added a short explanation beneath the personnel simulation button.
- Preserved the v0.97.30 championship-to-offseason repair.
- Preserved the championship-edition newspaper before Offseason.
- Preserved the matching transparent home-page, favicon, and web-app logo.
- Synchronized `v0.97.31` on the main page and persistent watermark.

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

Keep the existing `logos/` and `portraits/` folders in the repository.

## Updating the GitHub Repository

1. Extract the ZIP.
2. Upload `index.html` and `README.md` to the repository root.
3. Allow GitHub to replace the existing files with the same names.
4. The old `README.txt` is no longer used by Basketballverse updates and can be removed from the repository.

## Save Compatibility

Existing saved universes remain compatible. Saves that reached a crowned champion while still marked as being in the postseason are repaired when Offseason is opened.
