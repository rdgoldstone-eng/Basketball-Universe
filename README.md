# Basketballverse — v0.97.27

## Current Build
**v0.97.22 · Portrait Stability Fix**

### Changes in v0.97.22
- Keeps the expanded 1947 draft class at 78 documented real players.
- Stops the 1947 scouting list from rebuilding itself every second, which caused portrait flickering.
- Hides the initials/default portrait layer whenever a real portrait loads successfully.
- Shows initials only when the portrait file actually fails to load.
- Preserves the clean repository asset paths introduced in v0.97.18.

## Repository Structure

```text
Basketball-Universe/
├── index.html
├── README.md
├── portraits/
│   └── first_last.webp
├── logos/
│   ├── game/
│   │   └── basketballverse-logo.jpg
│   └── teams/
│       └── city-team-year.webp
└── files/
```

### Portrait naming
Player portraits use lowercase underscore-separated filenames, for example:
- `glen_selbo.webp`
- `walt_dropo.webp`
- `wataru_misaka.webp`

Future update ZIPs contain only `index.html` and `README.md`; static assets remain in the GitHub repository.


### v0.97.23
- Fixed team logos disappearing after game simulation by resolving historical artwork directly from `logos/teams/` on every render.
- Repaired `Open Playoffs` and `Begin Playoffs`, including the special 1946-47 BAA playoff initializer.


### v0.97.24
- Fixed the version badge changing while the game is running.
- The current build number and build label are now immutable after startup, so older historical patch hooks cannot overwrite them.
- Replaced repeated version-badge polling with a targeted observer on the startup badge.


### v0.97.26
- Fixed the real 1946-47 playoff-entry regression: an older capture-level click handler was calling a stale playoff function before the later repair could run.
- The 1947 postseason initializer now keys off `season.year` as well as `currentYear`, so it still works if the calendar year has already rolled forward at the end of the season.
- `Open Playoffs` and `Begin Playoffs` now point to the current global playoff entry function after each season render.
- Synced the startup version pill and the bottom-right build badge to the same current version.


### v0.97.27
- Fixed the blank Offseason Hub at Season Complete.
- Root cause: the newer checklist UI removes the original `offseasonStatus` element, while the old core renderer was returning before `initOffseason()` could run.
- Offseason state is now initialized before any legacy DOM checks.
- Existing saves already stuck at Season Complete with no offseason state are repaired automatically.
- Viewer should enter the offseason with Awards as the first task, followed by Retirements, Development, Draft Order, Draft, Re-signings, Free Agency, Roster Cuts, and Next Season.
