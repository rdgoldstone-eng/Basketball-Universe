v0.37.9 Basketball Universe — Drafted Rookie Ratings Fix

ROOT CAUSE
The interactive Draft Room was not using the same prospect-to-player conversion used by the original draft engine.
Prospects could enter the league without a properly realized OVR, potential, true potential, and skill profile.

FIXED
- Draft Room selections now use convertProspectToPlayer().
- Drafted players receive realized OVR/potential based on their draft-time prospect range and controlled variance.
- Rookie year remains the season beginning after that offseason draft (1984 draft -> 1984-85 rookie season).
- Draft results now show the player's actual realized OVR/POT instead of defaulting to 60.
- ROY is selected from actual rookie-season production, with a small ratings tiebreaker.
- If the currently completed season is still loaded, opening History recomputes that season's ROY using the corrected eligibility/profile data.

IMPORTANT PHILOSOPHY
Michael Jordan and Hakeem Olajuwon are NOT hardcoded to win 1984-85 ROY.
They should enter as elite prospects and usually be strong candidates, but another 1984 rookie can legitimately win if the alternate-universe season supports it.

GitHub update:
Upload index.html and README.txt over the current files and commit.
Existing saves continue to work, but players drafted before this fix keep the ratings they already received.
