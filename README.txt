Basketballverse
v0.91.35 · Player Portrait System

FOUNDATION
- Every player now has a stable portrait key based on player ID.
- Portraits follow the PLAYER, not the team.
- Trades therefore never require changing portrait ownership.
- Portrait artwork lives in /portraits and is not stored inside save data.
- Missing artwork gets a Basketballverse-styled fallback instead of a broken image.

FIRST UI INTEGRATION
- Player Profile: large portrait hero.
- Draft selection: compact portrait beside selectable prospects.
- The system is reusable for Free Agency, Trade Finder, awards, newspaper and
  Hall of Fame as the portrait library grows.

ASSET FORMAT
portraits/<normalized-player-id>.webp

IMPORTANT
This build establishes the portrait ENGINE. Individual historical-player art is
a separate asset library and can be added progressively without changing saves.

Retains all v0.91.34 systems.
