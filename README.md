# Basketballverse — v0.97.32

## Current Build

**v0.97.32 · Visible Sim Re-signings**

Basketballverse is a browser-based professional basketball universe simulator spanning the league's historical eras. Create or load a universe, choose a role, and let league history develop through simulation and alternate-history decisions.

## Changes in v0.97.32

- Fixed the missing Viewer-mode Sim Re-signings button.
- The button now appears near the top of the selected Re-signings task, directly below Open Re-sign Players.
- Fresh Re-signings stages no longer simulate automatically when the page is opened.
- Pressing Sim Re-signings processes league contracts exactly once and advances to Free Agency.
- Saves in which Re-signings already ran automatically show Continue to Free Agency instead, preventing duplicate contract processing.
- Removed the competing floating and hidden personnel controls.
- Preserved the championship-to-offseason repair and championship newspaper from v0.97.30.
- Preserved the matching transparent home-page, favicon, and web-app logo.
- Synchronized `v0.97.32` on the main page and persistent watermark.

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
4. The old `README.txt` is no longer used and can be removed from the repository.

## Save Compatibility

Existing saved universes remain compatible. A save that already displays completed Re-signings results will continue safely to Free Agency without running those contract decisions again.
