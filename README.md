# Basketballverse

Current build: **v0.97.21 · 1947 Real-Name Draft Repair**

## Repository structure

```text
Basketball-Universe/
├── index.html
├── README.md
├── portraits/
├── logos/
│   ├── game/
│   └── teams/
└── files/
```

## Asset paths

- Player portraits: `portraits/first_last.webp`
- Basketballverse logo: `logos/game/basketballverse-logo.jpg`
- Historical/team logos: `logos/teams/`
- Static audits/checklists/reference files: `files/`

## v0.97.21

- Fixes the 1947 scouting pool so it displays the 78 documented real draft names instead of the old procedural filler pool.
- Specifically eliminates malformed names such as `Damon undefined` and `Desmond undefined` from the 1947 class.
- Forces existing 1946-47 saves to replace the stale 1947 draft-class state with the authoritative historical list.
- Rebuilds the 1947 Draft Room available list from the same authoritative class when applicable.
- Keeps portrait naming as lowercase underscore-separated `.webp` files.

## Update workflow

Normal Basketballverse update ZIPs contain only `index.html` and `README.md`. Static assets stay in GitHub and should not be re-uploaded with every build.
