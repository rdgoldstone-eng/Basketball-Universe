# Basketballverse v0.95.11
## Portrait Mapping Repair

**CURRENT BUILD: v0.95.11**

Built directly from v0.95.10.

## Fix
v0.95.10 caused all roster portrait initials to become the same because an after-render
DOM scan was matching the wrong player object to multiple rows.

v0.95.11 removes that fuzzy row-text matching.

Each roster card now receives its portrait directly from the exact player object used
to build that card.

This restores correct initials for every player and keeps the single-folder lookup:

`portraits/julius_erving.webp`

## Test
Philadelphia 76ers > Team > Roster

Expected:
- Julius Erving = JE fallback if image cannot load, otherwise Dr. J image
- George McGinnis = GM
- Doug Collins = DC
- Henry Bibby = HB

No player should inherit another player's initials.
