v0.36.3 Basketball Universe — Season Header Fix

FIRST PLAYTHROUGH HOTFIX
- Fixed the top Season KPI staying on the prior season after offseason rollover.
- When currentYear moves from 1976 to 1977, the header now immediately changes from 1976-77 to 1977-78.
- The header now refreshes every time the game UI renders, so future season rollovers stay synchronized.
- Also refreshes role, controlled team and open-decision header values.

IMPORTANT
The screenshot showing October 15, 1977 and 0/82 games confirmed the 1977-78 season had actually started. The stale 1976-77 text was a display bug, not a failed offseason rollover.

Includes the v0.36.2 offseason navigation buttons.

GitHub update:
Upload index.html and README.txt over the current files and commit.
