v0.59 Basketball Universe — Navigation, Seeds & Autosave

USER-REQUESTED QUALITY-OF-LIFE UPDATE

1. CURRENT SIMULATION STAGE
The navigation now keeps a yellow outline around the part of the game where the universe currently is.

Examples:
- Regular Season -> Season is outlined
- Regular Season Complete / Playoffs -> Playoffs is outlined
- Completed postseason / offseason -> Offseason is outlined
- Draft stage -> Draft Room is outlined

This outline remains visible even when you open a different page such as History, so you always know where to return.

The normal filled/gold active button still shows the page you are currently viewing.
The yellow outline shows WHERE THE SIMULATION CURRENTLY IS.

2. PLAYOFF SEEDING
Playoff teams now display their original conference seed beside the team name.

Seeds:
- are stored when the playoff field is created
- remain attached to a team through later rounds
- appear in bracket series
- appear in the Next Game label
- appear in the playoff game log

Older saves that are already in the playoffs can reconstruct the seed map from their standings.

3. CHAMPION LOGOS IN HISTORY
History -> Champions now displays the champion's logo beside each champion.

The logo is resolved using the championship year, so the system is designed to show the identity/logo appropriate to that season instead of blindly using the franchise's current identity.

New champion records also store the franchise team ID for stronger relocation/rebrand lineage tracking.

4. TRUE AUTOSAVE / RETURN TO GAME
Basketball Universe now:
- autosaves every 15 seconds while active
- saves when the browser/app goes into the background
- saves on pagehide
- attempts a final save before unload
- automatically resumes the most recent saved universe when the game page is reopened

This is especially useful on iPhone, where Safari may suspend a tab when switching apps.

The compact mobile-save system from v0.58.1 remains in place, so embedded built-in logo artwork is not duplicated into localStorage.

TEST STATUS
JavaScript syntax validation passed.

The user's test universe successfully reached the 1990-91 season before this update with the historical expansion/crossroads system behaving normally.

GitHub update:
Upload index.html and README.txt over the current files and commit.
