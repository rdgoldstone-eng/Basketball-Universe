Basketballverse
v0.91.25 · Job Market Accept Fix

YES — THE ITEMS ON JOB MARKET ARE OFFERS
The Job Market tab was reading state.career.jobOffers, but its newer menu renderer
only displayed team/role text. It accidentally omitted the Accept and Decline controls
that existed in an older Career & Employment panel.

FIX
- Job Market now shows each open offer as a full card.
- Each offer shows team, role, source (vacancy/approach), and fit score.
- Added Accept Job and Decline buttons.
- Added Check for New Openings while unemployed.
- Dashboard shows number of currently open offers.

IMPORTANT FIRED-MODE FIX
v0.91.24 changes state.role to Viewer while unemployed.
The older GM/Coach job acceptance function restored the team but not state.role.
v0.91.25 fixes that:
- Accepting a job restores state.role to GM/Coach.
- controlledTeamId becomes the new team.
- career status becomes Employed.
- GM firing flags are cleared.
- normal team decisions and controls resume.
- user returns to the Season screen.

The existing offers in the user's current save should become actionable immediately.

This build keeps IndexedDB saves from v0.91.23 and true Viewer mode while unemployed from v0.91.24.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
