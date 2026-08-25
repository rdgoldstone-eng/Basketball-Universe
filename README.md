# Basketballverse v0.96.30
## Playoff Finals Transition Repair
**CURRENT BUILD: v0.96.30**

Built directly from v0.96.29.

Fixes the playoff error:
`TypeError: undefined is not an object (evaluating 'f.winnerId')`

Cause:
The older playoff transition code could set playoff round = 4 even when both
Conference Finals were not present/complete. That left the game labeled "NBA Finals"
without an actual NBA Finals series. The next playoff action then tried to read
`f.winnerId` from an undefined Finals object.

Fix:
- round 3 only advances when BOTH Conference Finals exist, are complete, and have winners
- the NBA Finals series is created only once
- round 4 no longer dereferences a missing or incomplete Finals object
- saves already stuck at round 4 with no Finals series automatically repair back to
  Conference Finals on load
- all v0.96.29 ABA, portrait, logo, merger and historical systems are retained
