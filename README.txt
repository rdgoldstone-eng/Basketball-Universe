Basketball Universe
v0.82.10 · Newspaper Timing Fix

WHAT WAS WRONG
The previous newspaper build searched the whole page for any button named "Continue."
The newspaper itself did not have its own Continue button. That could leave the
newspaper marked as pending until a completely unrelated Continue button appeared
at the end of the following season.

FIX
- The newspaper now has its OWN Continue button at the bottom.
- It appears immediately after Start Next Season.
- It displays the final edition for the season that just ended.
- Continue hides the newspaper and leaves you on the Season screen at Game 1.
- The newspaper does not remain pending through the season.
- The old page-wide generic Continue-button search is disabled.
- Existing saves with a stale pending-newspaper flag are repaired.
- If a save is already at Game 1 and the prior-season paper has not been acknowledged,
  it is restored as the opening screen.

EXPECTED FLOW
Finish offseason
→ Start Next Season
→ Season screen opens with prior-season newspaper
→ Continue to [new season]
→ newspaper closes
→ Game 1 controls are immediately visible

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root.
