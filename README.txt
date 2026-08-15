Basketballverse
v0.91.30 · Offseason Season Lock

BUG
A user was 41 games into the regular season, opened Free Agency, and accidentally
entered the offseason progression loop all the way to Start New Season.

ROOT CAUSE
Older Front Office / Offseason wrappers could still initialize or advance the
offseason workflow whenever those pages were opened. Free Agency also exposed a
"Finish Free Agency" progression button even during the regular season.

HARD RULE
The offseason workflow now exists ONLY when:
Season phase = Season Complete

That means:
- Regular Season: offseason locked
- Regular Season Complete / Playoffs: offseason locked
- Season Complete after Finals: offseason unlocked

IN-SEASON FREE AGENCY
Free Agency remains usable during the regular season for signing actual free agents.
But the page explicitly says "In-Season Free Agency" and contains NO:
- Finish Free Agency
- Roster Cuts progression
- Next Season progression
- offseason checklist advancement

SAFETY
- advanceOffseason() hard-blocks outside Season Complete.
- Offseason tab redirects to Season/Playoffs when locked.
- Start New Season hard-blocks unless the offseason is truly at Next Season.
- Re-signings and Roster Cuts cannot initialize during the regular season.
- Stale offseason objects from older builds are cleared when a regular-season save loads.

This build retains:
- Development-by-team dropdown
- historical salary cap/salaries
- luxury tax / repeater / apron rules
- IndexedDB saving
- trade finder and trade ownership fixes
- fired true Viewer mode and job market acceptance

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
