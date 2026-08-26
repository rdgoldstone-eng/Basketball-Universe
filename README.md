# Basketballverse v0.97.06
## Early League Membership & Logo Continuity

Built directly from v0.97.05.

### Early league volatility
Basketballverse now treats 1947-1951 as a volatile franchise environment.

Historical stress points are real crossroads, not forced outcomes:
- 1947: Cleveland, Detroit, Pittsburgh and Toronto face survival pressure.
- 1949: Providence and the Indianapolis Jets face survival/reorganization pressure.
- 1950: Anderson, Chicago, Denver, Sheboygan, St. Louis and Waterloo face post-merger pressure.
- 1951: Washington faces a major financial survival test.

A club's attendance, stability, fan support, record and recent weak seasons feed
a deterministic survival score. Strong alternate-history results can keep a
team alive even when it folded in real history.

When a team ceases operations:
- the franchise is removed from the active league
- its players enter a dispersal allocation / free-agent process
- the event is written to News and franchise history

### Historical league entries
The early league now has scheduled entry waves:
- 1947: Baltimore Bullets
- 1948: Fort Wayne Pistons, Indianapolis Jets, Minneapolis Lakers, Rochester Royals
- 1949: Anderson Packers, Denver Nuggets, Sheboygan Red Skins, Syracuse Nationals,
  Tri-Cities Blackhawks, Waterloo Hawks, Indianapolis Olympians

These entrants use the existing historical multi-team roster allocation engine
until dedicated incoming ABL/NBL roster packs are installed.

### Logo continuity fix
Some logos disappeared entering 1947-48 because the logo manifest correctly
ended the artwork in the franchise's real final season. That is wrong for an
alternate universe where the team survives.

v0.97.06 carries forward the last known historical logo for any identity that
still exists in the simulated league. For example, a surviving Toronto Huskies,
Cleveland Rebels, Detroit Falcons or Pittsburgh Ironmen continues using its 1946
logo rather than losing its artwork.

Historical logos are also explicitly re-applied during each early season transition.
