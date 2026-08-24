# Basketballverse v0.96.21
## ABA Franchise Health & Historical Obstacle UI
**CURRENT BUILD: v0.96.21**

Built directly from v0.96.20.

This update gives the ABA historical-obstacle system accumulated in-universe data.

Each ABA franchise now tracks:
- attendance and fan interest
- financial health / cash pressure
- ownership stability
- market strength
- arena quality
- star power
- annual business-history snapshots

The inaugural 1967-68 attendance environment seeds the starting business conditions.
After that, franchise health changes from Basketballverse results, star power, market
conditions and prior health rather than being forced to follow real history.

At each annual review, the game can now:
1. update every franchise's business health,
2. check that year's real historical pressure points,
3. attach the current Basketballverse health data to the event,
4. recommend stay / relocate / emergency financing / fold without forcing it,
5. feed the accumulated values into the 1976 dynamic merger negotiations.

A renderABAObstaclePanelV09621(year) UI renderer is included for the season/event screens.
The 1976 review invokes the dynamic merger model from v0.96.20.

Next update:
- wire annual reviews into the actual season-advance flow,
- create player/owner choices when an obstacle fires,
- persist accepted relocations/foldings into franchise identity/history,
- add the NBA-side vote and merger negotiation screen.
