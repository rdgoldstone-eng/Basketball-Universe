# Basketballverse — v0.97.45

## Current Build

**v0.97.45 · Historical Player Balance**

## Changes in v0.97.45

- Expands the 1947–1955 historical draft pools with documented players who appeared professionally, including notable undrafted players.
- Uses 396 verified historical draft/undrafted records across those founding-era classes.
- Rebalances early historical prospects by career tier so obscure late selections are not rated like superstars.
- Lowers procedurally generated fictional rookies to 43–57 initial overall with a maximum potential of 72.
- Stops adding visible numeric suffixes such as “2” or “3” solely because two players share a name.
- Assigns every fictional prospect a stable portrait key, portrait seed, and era year for the planned AI Headshot Generator.
- Repairs untouched 1947–1955 drafts in existing saves and rebalances young generated players without erasing completed league history.

## Expanded Historical Pool

- 1947: 65 professional players
- 1948: 70 professional players
- 1949: 66 professional players
- 1950: 47 professional players
- 1951: 26 professional players
- 1952: 36 professional players
- 1953: 33 professional players
- 1954: 31 professional players
- 1955: 22 professional players

## Installation

Replace the repository-root `index.html` with this version and replace the repository-root `README.md` with this file.

Keep the existing `portraits/`, `logos/`, and other asset folders in place.

## Portrait Workflow

Use Basketballverse Portrait Builder v0.4 for the newly added real players. The later AI Headshot Generator will use each real player's approved image as a reference and will create an era-appropriate person for fictional players using their stable portrait seed.
