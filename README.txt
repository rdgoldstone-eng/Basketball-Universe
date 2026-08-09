Basketball Universe
v0.82.2 · Offseason Workflow Repair

BLOCKER / USABILITY FIX
- Rebuilt the offseason menu so the CURRENT TASK is highlighted clearly.
- The main offseason button now says exactly what it is completing and what comes next.
- The current task opens automatically in the detail panel.
- Completed tasks can be reviewed and future tasks can be previewed without appearing broken.
- Awards now show directly inside the offseason screen, with a link to full Awards History.
- Retirements are processed when the Retirements stage is reached and now explicitly say "No retirements" when nobody retires.
- Development now explains what the stage does and shows each player's rating change.
- Draft Order now actually stores the generated order instead of silently discarding it.
- 1966–1984 drafts use a conference-worst-team COIN FLIP for picks #1/#2.
- Later eras use the game's draft-lottery system.
- Draft Order shows the mechanism and full first-round order, including traded pick ownership.
- Draft remains a separate Draft Room task; Viewer/Commissioner can use "Sim Rest of Draft" instead of clicking through every pick.
- Added a stronger save repair for malformed player/prospect names containing "undefined".
- Prevented Awards, Retirements, Development, and Draft Order from being processed twice when advancing.

TEST THIS BUILD
Start from the offseason and move through:
Awards → Retirements → Development → Draft Order.
You should see each current row highlight, meaningful content for every stage, and a visible coin flip or lottery result at Draft Order.

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root, replacing the previous files.
