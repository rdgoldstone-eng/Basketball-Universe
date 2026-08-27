# Basketballverse v0.97.18
## Clean Repository Structure

From this build forward, Basketballverse uses this repository layout:

Basketballverse/
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
    └── static checklists, audits, instructions, and reference files

### Naming standards

Player portraits:
- lowercase
- underscore between first and last name
- `.webp`
- Example: `clifton_mcneely.webp`

Team logos:
- lowercase
- hyphenated city-team-year
- `.webp`
- Example: `boston-celtics-1946.webp`

### Transition behavior

v0.97.18 treats the new folders as canonical, but temporarily falls back to old
locations while the GitHub repository is being reorganized:

- portraits first try `/portraits/`
- misplaced player portraits can temporarily fall back to `/logos/historical/`
- team logos first try `/logos/teams/`
- old team logos can temporarily fall back to `/logos/historical/`
- the Basketballverse brand logo first tries `/logos/game/`
- the old root `basketballverse-logo.jpg` remains a temporary fallback

Once the GitHub cleanup is complete, the legacy fallbacks can be removed.

### Future ZIP rule

Starting with v0.97.18, update ZIPs contain ONLY:

- `index.html`
- `README.md`

Portraits, team logos, the game logo, CSV checklists, and other static files stay
in GitHub and are not recopied into every update ZIP.
