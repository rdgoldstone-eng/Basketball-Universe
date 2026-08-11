Basketball Universe League
v0.89.1 · Next Season Readiness

FIX
The GM offseason could reach Next Season but refuse to continue without making
the reason obvious.

NEW NEXT SEASON TAB
The dedicated Next Season activity now shows an Opening-Night Checklist:
- Minimum roster (8 players)
- Opening-night maximum roster limit for the current era
- Rookie contracts

If something blocks the new season, the exact item is shown on screen with
shortcuts to Front Office, Free Agency, and Roster Cuts.

START NEXT SEASON
- The Start Next Season button now uses one explicit final-stage path.
- If the checklist passes, it calls the existing beginNextSeason() transition.
- If the transition throws an error, the actual error is shown in the Next Season tab.
- Other offseason stages keep the existing progression logic unchanged.

This build includes the dedicated offseason tabs from v0.89.

Upload index.html and README.txt to the GitHub Pages repository root.
