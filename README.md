# Basketballverse

## Current build
**v0.97.20 · 1947 Draft Pool Repair**

### What changed
- Repairs the 1947 draft class to use all **78 documented named selections** currently included in the historical source data.
- Removes the old procedurally generated filler prospects from the 1947 pool.
- Repairs already-saved 1946-47 universes when they are loaded, including an already-created 1947 Draft Room.
- Preserves already-completed 1947 draft results while rebuilding the remaining available player pool from the real historical class.
- Updates the visible build label so the running game clearly shows v0.97.20.
- Keeps the clean repository asset structure introduced in v0.97.18.

## Repository structure
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

## Asset naming
Player portraits use lowercase underscore-separated names, for example:
- `clifton_mcneely.webp`
- `andy_phillip.webp`
- `larry_bird.webp`

Team logos use the historical city-team-year naming format, for example:
- `boston-celtics-1946.webp`
- `baltimore-bullets-1947.webp`

## Updating GitHub
Future Basketballverse update ZIPs contain only `index.html` and `README.md`. Replace those two files in the repository. Keep `portraits/`, `logos/`, and `files/` in place.
