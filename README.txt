v0.37.7 Basketball Universe — Finals MVP Stat Fix

ROOT CAUSE FOUND
Normal simulated playoff games were generating box scores but were NOT adding those box scores to playoffPlayerStats.
Only Watch Game was doing that.

That meant:
- Sim Next Game / Finish Series / Finish Round could complete the Finals.
- But Finals player totals stayed empty.
- The Finals MVP selector therefore had no eligible candidates.
- History correctly asked for a Finals MVP, but none existed.

FIXED
- Every normally simulated playoff game now adds its box score to playoffPlayerStats.
- Finals games now accumulate finalsGp, finalsPts, finalsReb and finalsAst.
- Finals MVP is selected from actual Finals production.

SAVE REPAIR
- For older completed seasons where those accumulated stats are missing, the game can reconstruct the current Finals MVP directly from the stored Finals game box scores.
- Opening History on a currently completed season can therefore repair the missing Finals MVP when the Finals games are still in the save.

GitHub update:
Upload index.html and README.txt over the current files and commit.
Existing saves should continue working.
