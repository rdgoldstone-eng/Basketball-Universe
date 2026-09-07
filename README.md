# Basketballverse — v0.97.33

## Current Build

**v0.97.33 · One-Conference Finals Repair**

Basketballverse is a browser-based professional basketball universe simulator spanning the league's historical eras. Create or load a universe, choose a role, and let league history develop through simulation and alternate-history decisions.

## Changes in v0.97.33

- Fixed the 1947–48 postseason becoming stuck when the bracket has no Western Conference series.
- A conference with at least two remaining teams now receives a valid conference-final series even when the older six-team bracket builder omitted it.
- A one-team conference receives a bye into the league Finals.
- When the league truly has only one conference, its final two survivors now play a valid league championship series instead of waiting for an impossible second conference champion.
- Completed one-conference series now crown the champion and advance normally to the championship newspaper and Offseason.
- Existing saved universes already stuck at this point are repaired automatically when loaded; a new universe is not required.
- Preserved the visible Viewer Sim Re-signings control and duplicate-processing protection from v0.97.32.
- Preserved the championship newspaper transition and matching transparent home-page, favicon, and web-app logo.
- Synchronized `v0.97.33` on the main page and persistent watermark.

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

Existing saved universes remain compatible. On load, v0.97.33 checks a stalled playoff bracket and supplies the correct path based on the available conferences: a rebuilt missing conference final, a conference bye, or a promoted one-conference league Finals.
