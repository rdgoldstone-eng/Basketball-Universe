# Basketballverse v0.92.02 — Owner Draft Button Fix

Built directly from v0.92.01.

## Exact bug fixed
The Draft Room already recognized the Indiana Pacers as the controlled team and displayed:
- Indiana Pacers is on the clock
- YOUR PICK
- Draft buttons

However, pressing Draft called the older `gmDraftPlayerV0881()` handler. That handler required `isHumanGMV084()`, which returns true only for GM mode. Therefore Owner mode displayed the correct pick but rejected the button press with:
`Your team is not currently on the clock.`

v0.92.02 removes that obsolete GM-only requirement. The Draft button now uses the game's real `isUserDraftPick()` check, which already supports both GM and Owner.

## Package
- index.html
- README.md
- basketballverse-logo.jpg
- historical Raptors and Grizzlies logo assets

All Owner systems from the previous builds remain included.
