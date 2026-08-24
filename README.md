# Basketballverse v0.96.17
## 1967 Rivalry Era — NBA / ABA Selection
**CURRENT BUILD: v0.96.17**

Built directly from v0.96.16.

New-game behavior:
- For the 1967 era, a League dropdown appears directly after the era selector.
- League choices: NBA or ABA.
- Selecting ABA filters the team selector to the 11 inaugural 1967-68 ABA franchises.
- Selecting NBA restores the era's existing NBA team choices.
- For every other starting era, the League selector is hidden and NBA remains the default.
- The selected league is exposed through getSelectedLeague() / isABAUniverse() for the next ABA simulation systems.

1967 ABA teams:
Eastern: Indiana Pacers, Kentucky Colonels, Minnesota Muskies, New Jersey Americans, Pittsburgh Pipers.
Western: Anaheim Amigos, Dallas Chaparrals, Denver Rockets, Houston Mavericks, New Orleans Buccaneers, Oakland Oaks.

This build establishes the startup-selection layer. Next we can wire the ABA choice into
its own standings, schedule, rules, playoffs, awards, transactions and background NBA simulation.
