# Basketballverse

**Current build:** v0.97.19 — Expanded 1947 Draft Pool

Basketballverse is a historical basketball universe simulation that begins in the BAA/NBA's early years and allows league history to branch into an alternate timeline.

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
    └── checklists, audits, and reference files
```

## Asset naming

- Player portraits: lowercase `.webp` using underscores, for example `larry_bird.webp` and `clifton_mcneely.webp`.
- Team logos: lowercase `.webp` using hyphens and the historical year, for example `boston-celtics-1946.webp`.
- Basketballverse game logo: `logos/game/basketballverse-logo.jpg`.

## v0.97.19

- Expanded the 1947 historical draft pool to 78 documented players across 10 rounds.
- Preserves documented historical players instead of inventing players simply to fill draft slots.
- Scouting and Draft Room use the expanded 1947 class.
- Player portraits continue to resolve through the canonical `portraits/first_last.webp` convention.
- Canonical repository asset paths remain `portraits/`, `logos/game/`, `logos/teams/`, and `files/`.

## Updating the game

Normal Basketballverse update ZIPs contain only:

- `index.html`
- `README.md`

Do not replace or re-upload the `portraits`, `logos`, or `files` folders when installing a normal game update.
