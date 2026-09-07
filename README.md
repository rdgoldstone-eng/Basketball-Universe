# Basketballverse — v0.97.36

## Current Build

**v0.97.36 · Browser-State Playoff Repair**

Basketballverse is a browser-based professional basketball universe simulator spanning the league's historical eras. Create or load a universe, choose a role, and let league history develop through simulation and alternate-history decisions.

## Changes in v0.97.36

- Fixed the actual browser-only failure that prevented the 1947–48 playoff repair from running.
- Basketballverse stores its live game state in the script-level `state` variable. The previous repair incorrectly required `window.state`, which does not exist in a real browser.
- Removed that invalid guard from the 1947–48 playoff initializer and its supporting early-playoff repairs.
- A save already stuck at Conference Finals with zero games and zero teams now has its empty bracket replaced automatically.
- The 1947–48 season now qualifies the top three teams from each division for the historically correct six-team BAA postseason.
- The two division champions play a best-of-seven semifinal; the second- and third-place cross-division series and runners-up semifinal are best-of-three; the BAA Finals are best-of-seven.
- Empty playoff rounds can no longer continue bypassing the historical bracket repair.
- The season is recognized from the saved `season.year`, even if the live calendar has already moved into 1948.
- Preserved playoff entry buttons, team logos, championship newspaper, Offseason transition, Viewer Sim Re-signings control, and transparent web-app icons.
- Synchronized `v0.97.36` on the main page and persistent watermark.

## Regression Test

The repaired code was tested under real browser state semantics:

- `state` exists as a script-level variable.
- `window.state` does not exist.
- The 1947–48 save begins at an empty Conference Finals round.
- The repair creates six playoff seeds and three opening series.
- The postseason advances through five total series and reaches `Season Complete` with a champion.

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

Existing saved universes remain compatible. v0.97.36 replaces only a completely empty or untouched 1947–48 playoff bracket. Any postseason containing played games or completed results remains untouched.
