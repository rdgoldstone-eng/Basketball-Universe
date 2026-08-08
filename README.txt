v0.37.8 Basketball Universe — Awards Eligibility Fix

ROOT CAUSE
Rookie of the Year eligibility was simply age <= 23. That allowed the same young player to win ROY in multiple seasons.

FIXED
- ROY now requires rookieYear to exactly match the current season.
- Draft Room rookies are assigned rookieYear based on their actual draft/entry season.
- Deferred draft-rights players become ROY eligible in the season they actually join.
- The starting 1976-77 universe now seeds the actual 1976 rookie group rather than treating every young player as a rookie.
- Existing history removes impossible repeated ROY entries when they can be identified from rookieYear data.

OTHER AWARD CLEANUP
- Sixth Man now requires a meaningful bench role: non-starter, at least 20 games, roughly 12-30 MPG.
- DPOY now weights steals, blocks, rebounding and defense rating rather than leaning mostly on OVR.
- Repeated DPOY winners are still possible if a player genuinely remains the best defensive performer.

DISPLAY
- History season labels now show full season format, e.g. 1983-84 instead of just 1983.

GitHub update:
Upload index.html and README.txt over the existing files and commit.
Existing saves should continue working.
