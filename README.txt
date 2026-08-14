Basketballverse
v0.91.22 · Save Reliability Fix

PROBLEM
Long-running universes can stop updating in browser storage even though the game
continues running. Mobile Safari/localStorage has a limited quota, and raw
simulation/UI caches can make a save grow much larger than the actual permanent
league history requires.

FIX
- Every save now gets a durable lastSuccessfulSaveAt marker.
- Basketballverse performs a read-after-write verification before saying Autosaved.
- The Saved Universes card timestamp now reflects the verified durable write.
- Save size (KB) is shown in the autosave/status information.
- Added a Save Now button that uses the exact same verified save path.
- If saving fails, the header says SAVE FAILED and the game shows the actual error.

STORAGE OPTIMIZATION
Canonical history is preserved:
- season history
- champions
- draft history
- franchise history
- newspapers
- players/teams/contracts
- career history

Only large/recreatable data is reduced:
- Trade Finder offer cache
- current Trade Machine selections
- old raw box-score payloads beyond the most recent 80
- oversized recent-game arrays
- old resolved decision logs
- very old news beyond a large retained archive
- old transition-error logs
- excessive transaction/UI caches

This is intended to keep multi-decade universes saveable on iPhone/Safari.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
