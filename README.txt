Basketballverse
v0.91.24 · Fired True Viewer Mode

ROOT CAUSE
The GM firing code correctly set:
- state.gmCareer.status = "Fired"
- state.career.status = "Unemployed"
- controlledTeamId = null

But it left:
- state.role = "GM"

Many older Basketballverse systems check state.role directly instead of the
newer viewerMode() helper. So after being fired, those systems still treated
the player like an active GM.

FIX
After firing/unemployment:
- state.role becomes Viewer
- controlledTeamId remains null
- state.career.role preserves the actual profession (GM/Coach/etc.)
- state.career.status remains Unemployed
- all unresolved team decisions are closed
- new team/injury decisions are blocked
- simulation runs exactly like Viewer mode
- UI shows "GM · Unemployed", "Viewer", and "No Team"

NEW JOB
When a career job is accepted:
- the saved career role is restored to state.role
- the new controlled team is restored
- employment returns to Employed
- GM status returns to Employed

EXISTING FIRED SAVES
v0.91.24 repairs them automatically on load/render. You do not need to get fired again.

This build keeps the IndexedDB save system from v0.91.23.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
