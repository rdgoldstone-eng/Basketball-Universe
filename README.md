# Basketballverse v0.96.35
## Early Draft Room Recovery

Fixes the next blocker found after the repaired 1947 postseason:
- early historical draft class exists but Draft Room can open with an empty/stale draftRoom
- Draft stage can then have no prospects and no usable path forward
- Viewer mode now has an explicit Sim Rest of Draft control
- completed drafts always expose Continue Offseason

For 1947-1976, if the offseason is at Draft and the room is empty before any picks
have been made, the game rebuilds the Draft Room directly from the loaded historical
class for currentYear + 1.

No new universe is required.
