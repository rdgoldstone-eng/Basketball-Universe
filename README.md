# Basketballverse v0.96.25
## Dynamic Post-Merger NBA Alignment & Schedule
**CURRENT BUILD: v0.96.25**

Built directly from v0.96.24.

After the interactive 1976 merger/dispersal event finishes, Basketballverse now rebuilds
the NBA around the actual franchises admitted from the ABA.

Implemented:
- admitted ABA franchises are inserted into the NBA
- conferences are assigned from geography, then balanced to within one team
- four NBA divisions are rebuilt: Atlantic, Central, Midwest, Pacific
- the alignment is stored in the universe for history/save data
- a new schedule generator targets 82 games per team
- every opponent is scheduled home and away first
- remaining games prioritize division opponents, then conference opponents
- the resulting alignment is displayed after the merger is completed
- transition state is created for the 1976-77 NBA preseason

Historical grounding:
The real 1976 merger produced a 22-team NBA after Denver, Indiana, New York and San Antonio
were admitted. NBA.com's 1976-77 season review confirms the 22-team league and a restructured
12-team playoff field. Basketballverse uses that as the historical baseline but rebuilds
alignment dynamically if a different number or identity of ABA franchises joins.

Next:
- make playoff qualification dynamically preserve the 1976-77 12-team structure where feasible
- connect the generated schedule to the existing game simulation
- make merged ABA rosters/transactions visible everywhere in the NBA UI
- resume the 1967-76 ABA season simulation loop and player-development/rating work.
