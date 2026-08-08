v0.37.3 Basketball Universe — Season Transition Fix

FIXED
- Hardened the offseason -> next season transition after Viewer testing got stuck trying to begin 1978-79.
- Noncritical systems (development, staff, ownership, coaching, draft-pick maintenance) can no longer prevent the next season from starting if one of them errors.
- Added a fallback season initializer so the league always reaches the next October with standings reset to 0-0.
- Start Next Season now gives visible button feedback while transitioning.
- Any bypassed background transition error is recorded internally for later debugging instead of trapping the save.

Viewer remains simple:
- No team control
- No decision interruptions
- Normal season selector
- Normal playoff controls
- Normal offseason flow

GitHub update:
Upload index.html and README.txt over the current files and commit.
Your existing save should continue; you should not need to restart.
