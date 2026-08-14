Basketballverse
v0.91.21 · Traded Draft Pick Ownership Fix

BUG
A GM traded with Atlanta for the #1 pick, but Atlanta still made the selection.

CAUSE
Different systems were reading different draft-pick ownership fields. The trade
could change ownerTeamId while the Draft Room still used teamId/original-team data.

FIX
- Draft-pick trades update all current-ownership fields together.
- originalTeamId stays separate for history and pick projection.
- Legacy teamId is synchronized to the CURRENT owner.
- Draft order is repaired from current ownership before rendering.
- The current selection is checked again immediately before a draft action.
- Existing saves with an active draft are repaired on load.

RESULT
If Atlanta trades the #1 pick to your team before the selection, your team owns
and uses the #1 pick. Atlanta remains only the pick's original franchise.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
