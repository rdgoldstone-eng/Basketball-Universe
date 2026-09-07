# Basketballverse — v0.97.34

## Current Build

**v0.97.34 · 1947–48 Playoff Field Repair**

Basketballverse is a browser-based professional basketball universe simulator spanning the league's historical eras. Create or load a universe, choose a role, and let league history develop through simulation and alternate-history decisions.

## Changes in v0.97.34

- Fixed the 1947–48 season creating an empty playoff field when neither conference had the six teams required by the later-era bracket builder.
- The early-league postseason now qualifies the six best clubs in the full league standings, or every surviving club when fewer than six remain.
- First-round and semifinal byes now adjust automatically to fields containing two through six teams.
- A two-team league begins directly in the Finals; three- and four-team fields begin in the semifinals; five- and six-team fields receive a valid first round.
- Existing 1947–48 saves with an empty playoff state are rebuilt automatically when loaded, without restarting the universe.
- The repaired bracket advances through every round, crowns a champion, displays the championship newspaper, and reaches Offseason normally.
- Preserved the one-conference Finals completion repair from v0.97.33.
- Preserved the visible Viewer Sim Re-signings control and duplicate-processing protection.
- Preserved the matching transparent home-page, favicon, and web-app logo.
- Synchronized `v0.97.34` on the main page and persistent watermark.

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

Existing saved universes remain compatible. If a 1947–48 save already contains an empty playoff state, v0.97.34 replaces only that empty bracket with the flexible early-league field. Played playoff games and completed postseason data are not reset.
