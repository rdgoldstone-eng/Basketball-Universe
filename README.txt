Basketballverse v0.91.31 · Historical Salary Demand Fix

BUG: Bill Cartwright could ask $26M in 1984-85 despite a $3.6M cap.

CAUSE: stale free-agent/re-signing demand fields from the game's former ~$100M
economy survived the historical salary conversion.

FIX:
- Era salary demand is authoritative everywhere.
- Legacy/cached demand fields are repaired on load and render.
- Free agency, re-signings and contract offers use the 1984-85 scale.
- 1984-85 superstar market reference is about $2.34M; ordinary players scale below it.
- Existing saves are repaired automatically.

Retains all v0.91.30 systems.
