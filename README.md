# Basketballverse — v0.97.35

## Current Build

**v0.97.35 · Historical 1948 BAA Playoffs**

Basketballverse is a browser-based professional basketball universe simulator spanning the league's historical eras. Create or load a universe, choose a role, and let league history develop through simulation and alternate-history decisions.

## Changes in v0.97.35

- Restored the historically correct six-team postseason for the 1947–48 BAA season.
- The top three clubs from the Eastern Division and top three from the Western Division now qualify.
- The two division champions play a best-of-seven semifinal.
- The second-place clubs meet cross-division in a best-of-three opening series, as do the third-place clubs.
- The two opening-series winners meet in a best-of-three semifinal, with that winner advancing to the best-of-seven BAA Finals.
- Fixed the season-identification bug that checked the moving calendar year instead of `season.year`, which caused some 1947–48 saves to bypass the repair entirely.
- Existing empty or untouched 1947–48 playoff states are rebuilt automatically without restarting the universe.
- Preserved already-played postseason games; the repair will not reset a bracket after playoff results exist.
- Preserved the championship newspaper, Offseason transition, Viewer Sim Re-signings control, and transparent Basketballverse web-app icons.
- Synchronized `v0.97.35` on the main page and persistent watermark.

## Historical Reference

The real 1948 BAA Playoffs included six teams. Philadelphia defeated St. Louis 4–3 in the division-champions semifinal, Baltimore advanced through the shorter side of the bracket, and Baltimore defeated Philadelphia 4–2 in the BAA Finals.

Basketballverse uses the historical structure while allowing the qualifying teams and winners to follow the saved universe's standings and results.

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

Existing saved universes remain compatible. v0.97.35 replaces only an empty or completely untouched 1947–48 playoff bracket. If a playoff game has already been played, that postseason data is preserved.
