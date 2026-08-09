v0.62.1 Basketball Universe — Draft & Logo Fixes

FIXED: UTAH JAZZ LOGO AFTER RELOCATION
The 1979 New Orleans -> Utah relocation no longer leaves the Jazz without a logo.
Until the full dedicated Utah-era logo pack is added, Utah inherits the embedded historical Jazz artwork rather than falling back to blank/generic art.

FIXED: DALLAS MAVERICKS EXPANSION LOGO
Dallas now has an embedded classic Mavericks PNG beginning with the 1980 expansion identity.
Historical expansion teams now resolve their historical logo immediately when created.

RELOCATION / EXPANSION ASSET FIX
applyIdentityToTeam() and historical expansion creation now actively resolve:
1. historical PNG
2. identity artwork
3. generated fallback
instead of assigning null and hoping a later render fixes it.

FIXED: HISTORICAL DRAFT AI
The Draft Room AI had a major bug:
estimateProspectValue() looked for OVR/rating but did not read the historical draft-class "prospect" grade.
That meant elite historical prospects could effectively be valued near 60 by the AI.

This is why outcomes such as Michael Jordan falling to #17 were possible.

Draft AI now correctly uses:
- draft-time prospect grade
- draft-time ceiling range
- historical draft-night reputation
- positional fit
- age
- scouting uncertainty
- small randomness

DRAFT-NIGHT REPUTATION GUARDRAILS
Historical reality still does NOT force the exact real draft order.

However, universally elite prospects can no longer suffer absurd slides.

Examples:
- Patrick Ewing in 1985 is treated as a true consensus #1-level prospect. The alternate team holding #1 may choose him regardless of which real team owns that pick, but he should not randomly fall to #5.
- Michael Jordan in 1984 is not hardcoded to #3, but his draft-night standing makes a fall into the middle of the first round unrealistic. His reasonable range is kept near the top.
- Hakeem Olajuwon and Sam Bowie similarly retain their actual draft-night stature without forcing their exact real-world teams/order.

PHILOSOPHY
Real-world draft position is now used as evidence of contemporary consensus, NOT hindsight.

A future star who was genuinely viewed as a late pick still remains a late-pick type prospect.
A player who was universally regarded as an elite prospect cannot be buried simply because the AI likes positional fit.

LEGACY RUN-DRAFT FIX
The older automatic draft path also incorrectly treated draft-order objects as raw team IDs. That path has been repaired and now uses the same prospect valuation philosophy.

EXISTING SAVE NOTE
Your existing alternate history is not rewritten. If Jordan already went #17 and Ewing #5 in that universe, those events remain part of that save.
The corrected draft logic applies to future drafts and to newly created universes.

EXPANSION ERA
The long regression test has now successfully reached the Expansion Era. The next major content phase can focus on 1988-2003 Historical Crossroads after these fixes are verified.

GitHub update:
Upload index.html and README.txt over the current files and commit.
