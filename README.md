# Basketballverse v0.96.31
## Accurate 1947 BAA Playoff Repair
**CURRENT BUILD: v0.96.31**

Built directly from v0.96.30.

The remaining playoff lock was not just a missing null-check. The root cause was the game
using a later 12-team playoff structure in the inaugural 1946-47 BAA season.

The 1946-47 league has 11 teams split 6 East / 5 West. The old engine expected six playoff
teams PER conference, so the five-team West could not create a valid opening bracket. That
eventually produced a Conference Finals result on one side while no valid Finals opponent
could be created.

v0.96.31 adds the actual 1947 BAA structure:
- six playoff teams total: top three in each division
- East #1 vs West #1 in a best-of-seven "division champions" semifinal
- East #2 vs West #2 in best-of-three
- East #3 vs West #3 in best-of-three
- the two short-series winners play a best-of-three semifinal
- that winner meets the division-champions-series winner in a best-of-seven BAA Finals

Legacy save repair:
If a 1946-47 save is already stuck in the old malformed Conference Finals / NBA Finals state,
the game detects it on load. Because the old bracket is structurally invalid and cannot be
continued reliably, Basketballverse rebuilds ONLY that season's postseason bracket from the
saved regular-season standings using the correct 1947 format. Regular-season results, rosters,
portraits, team history and the rest of the save are preserved.

All later-era playoff logic remains unchanged.
