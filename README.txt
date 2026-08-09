v0.64 Basketball Universe — Season Chronicle & Era Accuracy

SEASON CHRONICLE
A newspaper-style season recap is created at the start of the next season, after the offseason draft is complete.

It includes:
- League champion and runner-up
- Finals MVP
- MVP
- Rookie of the Year
- Defensive Player of the Year
- Sixth Man
- #1 overall draft selection
- Major franchise events such as relocations, serious relocation reviews, expansion, rebrands, arena/ownership events
- Current East/West balance and that season's playoff format

The latest edition appears on the Season page.

PLAYOFF ERA FIX
1976-77 through 1982-83:
- 12 playoff teams
- 6 per conference
- top two seeds receive first-round byes
- first round best-of-3

1983-84 through 2001-02:
- 16 playoff teams
- 8 per conference
- first round best-of-5

2002-03 onward:
- 16 playoff teams
- first round best-of-7

This fixes the 12-team playoff field incorrectly continuing into 1991.

DRAFT SIZE FIX
Draft Room now has:
- one first-round pick for every active franchise
- one second-round pick for every active franchise

So a 25-team league receives 25 first-round picks and 25 second-round picks.

Historical classes that are not deep enough are supplemented only at the bottom of the class with uncertain generated late-round prospects. The historical top of the class is not changed.

DRAFT LOTTERY
Era-aware draft order is now used.

Through 1984:
- conference-worst coin-flip system for picks 1 and 2

1985:
- equal-odds lottery for all non-playoff teams

1986-1989:
- equal-odds lottery determines the top three
- remaining non-playoff teams pick in inverse record order

1990-1993:
- weighted lottery for the top three

1994-2018:
- weighted top-three lottery using the historical odds structure

2019 onward:
- four lottery selections with flattened modern odds

The second round is reverse regular-season record.

AUTOMATIC ALIGNMENT
In Viewer, Owner, GM, Coach and Player modes:
- conferences automatically rebalance as the league expands or relocates
- East and West stay as even as possible
- the game may cross the user's preferred Mississippi River boundary when needed for balance
- divisions are assigned and kept as even as possible
- pre-2004 uses two divisions per conference
- 2004 onward uses three divisions per conference

Commissioner mode remains manual and does NOT auto-realign.

EXPANSION LOGOS
Visible embedded PNG identity marks are now guaranteed for:
- Charlotte Hornets
- Miami Heat
- Orlando Magic
- Minnesota Timberwolves
- Toronto Raptors
- Vancouver Grizzlies
- Memphis Grizzlies
- New Orleans Hornets
- Charlotte Bobcats

This also fixes older saves whose expansion identities existed with logo:null.

CHAMPION RELOCATION GUARDRAIL
Winning now materially improves:
- attendance
- fan support
- franchise stability
- relocation pressure

A reigning champion receives a very large relocation-resistance adjustment.
A recent champion or Finals participant also receives protection.

This specifically prevents outcomes like Vancouver winning the championship and then casually moving to Memphis one year later. Such a move would now require an extraordinary ownership/arena crisis rather than the normal relocation threshold.

All v0.63 Expansion Era crossroads remain.
All v0.62 draft-prospect and logo fixes remain.
Multi-universe saves and Season Home remain.

Recommended regression test:
Use the saved universe you have already advanced into the LeBron era. Continue a few seasons and verify the Chronicle, 16-team playoffs, 2-round draft, lottery, alignment, expansion logos, and relocation behavior.
