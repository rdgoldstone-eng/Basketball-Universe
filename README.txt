Basketball Universe
v0.82.4 · Draft Engine Hard Fix

WHY THIS BUILD EXISTS
The previous Draft Room fixes still depended on the original draft-pick execution path. Since the buttons could still appear to do nothing, this build bypasses that path instead of patching it again.

FIXES
- Replaced the visible Draft Room simulation buttons with explicitly bound JavaScript controls.
- "Sim This Pick" now uses a new self-contained draft-pick executor.
- "Sim Rest of Draft" uses the same executor in a fast loop.
- The new executor handles team resolution, prospect choice, player creation, contracts, deferred draft rights, results, pick advancement, and completion directly.
- Optional transaction/history logging can no longer freeze the core draft.
- Added visible Draft Status text directly under the buttons.
- If a pick fails, the screen now reports the actual failure instead of appearing to do nothing.
- A stuck pick counter is detected and stops safely.
- Existing malformed prospect names are repaired before simulation.

TEST
Open Draft Room and look under the buttons. It should say "Draft engine ready."
Tap "Sim This Pick." The status line must either show the completed pick or a specific error.
Then tap "Sim Rest of Draft."

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root.
