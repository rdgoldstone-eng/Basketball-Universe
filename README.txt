Basketballverse
v0.90.7 · Injury Decision Fix

BUG FROM SCREENSHOT
ReferenceError: Can't find variable: injuryEventId

CAUSE
The injury decision system correctly created an injuryKey variable, but the
final addRoleDecision() call accidentally referenced a nonexistent variable
named injuryEventId instead of passing injuryKey into the injuryEventId field.

FIX
- Corrected injury decision metadata to:
  injuryEventId: injuryKey
- Added a safety wrapper so an injury-decision issue can be logged without
  stopping the regular-season simulation.
- Added a dashboard role sync so Role / Control labels cannot disagree after
  a fresh universe or load.

This build keeps the official Basketballverse logo.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
