# Basketballverse v0.95.00
## Era Framework + Universal Portrait Engine

**CURRENT BUILD: v0.95.00**

## Era framework
Basketballverse now has a formal registry for all planned startup eras:
- 1946 — The Founding Era
- 1967 — ABA Rivalry Era
- 1976 — Merger Era
- 1988 — Expansion Era
- 2003 — Realignment Era
- 2019 — Play-In Era
- 2026 — Current Day

### Current playable data packs
- 1976 — complete existing historical universe
- 2026 — complete existing current-day snapshot

1946, 1967, 1988, 2003, and 2019 are now registered as separate era data packs to be installed next. The game will no longer silently load the 1976 teams/players when one of those unfinished start years is selected.

## Universal Player Portrait Engine
All historical and created-player images now have one lookup path:
1. career/created-player uploaded portrait
2. explicit player portrait/photo/headshot
3. historical portrait pack lookup by player ID / portrait key / player name
4. initials fallback

Existing Basketballverse portrait helpers now route through this universal resolver. This means future portrait packs only need to register each image once for every compatible screen to use it.

### Portrait-pack API
Future era/draft portrait packs can call:
- `registerHistoricalPortraitPackV09500({...})`
- `applyPortraitPackToPlayersV09500()`

This is the foundation for installing the historical era snapshots and portrait packs one era/class at a time without rewriting the UI for every picture.
