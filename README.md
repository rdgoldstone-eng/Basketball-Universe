# Basketballverse — v0.97.23

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
