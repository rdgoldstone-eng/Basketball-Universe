Basketballverse v0.91.43 · Historic Newspapers

PORTRAITS ARE NOW A CORE PLAYER UI ELEMENT
Portraits are automatically added/re-added on:
- Team roster
- Player Profile
- Draft selection
- Draft History
- Free Agency
- Trade Machine
- Trade Finder
- Injury Report / Health
- League stats and player leaderboards
- All-Time career leaderboards
- Player Encyclopedia
- Awards History
- Hall of Fame / Hall watch
- Transaction lists when a player can be identified

A MutationObserver also catches player rows produced by older render wrappers,
so portraits survive screen refreshes and rerenders.

PORTRAIT MASTER LIST
portraits/portrait-manifest.json contains 54 UNIQUE player
portrait filenames from Batches 1-4.

From Batch 5 onward, portrait creation should compare against this master list
first so we do not waste batches generating players who already have artwork.

LONG-TERM GOAL
Every historical player in the Basketballverse database can eventually receive a
portrait. Generated fictional players continue to use the fallback portrait until
a generated-player portrait system is expanded.

Retains all v0.91.41 simulation, financial, roster and contract systems.


v0.91.43 adds historically aware newspaper headlines. Final Editions now recognize first titles, repeat champions, three-peats, 4+ title streaks, title droughts, franchise championship totals, MVP career totals, consecutive MVP streaks, and new all-time MVP records using the simulated universe history.
