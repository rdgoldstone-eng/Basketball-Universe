# Basketballverse v0.95.12
## Clean Single Portrait System

**CURRENT BUILD: v0.95.12**

This build removes the stacked portrait patches from v0.95.06 through v0.95.11.

Instead of adding another renderer, v0.95.12 changes the game's ORIGINAL v0.91.35
portrait functions directly.

### Permanent portrait rule

Player portraits live in:

`portraits/`

The filename is based on the player's name:

- Julius Erving → `portraits/julius_erving.webp`
- Bill Walton → `portraits/bill_walton.webp`
- Pete Maravich → `portraits/pete_maravich.webp`

The old system used the player's internal ID first. That was the core mismatch:
uploading `julius_erving.webp` could never work if the game was requesting an
ID-based filename.

### Exact test

Keep this file in GitHub:

`portraits/julius_erving.webp`

Then load:

Philadelphia 76ers → Team → Roster

The original roster renderer now requests:

`./portraits/julius_erving.webp?bv=09512`

No DOM scanning, no fuzzy player matching, and no replacement roster renderer is used.
