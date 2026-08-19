# Basketballverse v0.91.85 — Player In-Season Decision Loop

## In-season Player decisions fixed
Player-mode career decisions now trigger from actual season progress instead of depending on a specific Career-page render path.

Basketballverse checks the controlled player's games played using multiple sources:
- Player Career season totals
- player stats
- simulator stats

This prevents event droughts when one stat path is not updated.

## Decision cadence
After the first few games, Player mode targets roughly one meaningful decision every 4–7 player games.

Only one decision can be pending at a time, so decisions do not pile up.

## Decision types
The regular-season loop can now produce:
- Media Availability
- Meeting With the Coach
- Locker Room Moment
- Heavy Legs / workload decision
- Front Office Check-In
- Team leadership situation

Choices affect the established Player systems such as:
- Coach relationship
- Front Office relationship
- teammate/fan relationship
- confidence
- morale
- energy
- development
- chemistry
- loyalty
- ambition
- reputation

## Season screen
Pending Player decisions now appear prominently at the TOP of the Season screen with the actual response buttons.

You no longer have to go looking through Career to discover that an event is waiting.

## Player Career notice
If a decision is pending while viewing Player Career, a Decision Waiting notice directs you back to Season.

## Existing saves
If an existing Player save is already several games into the season, v0.91.85 adjusts the initial decision timer so you do not have to wait another long stretch before seeing the system work.

## Version
v0.91.85 · Player In-Season Decision Loop
