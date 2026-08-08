v0.37.6 Basketball Universe — Finals History Fix

FIXED
- Finals runner-up was being read from an obsolete playoff state object.
- Finals MVP was being chosen AFTER league history was already saved.
- Championship history now waits until the Finals are fully resolved, then stores:
  * Champion
  * Runner-up
  * Finals MVP

SAVE REPAIR
- Existing saves with a completed current season will automatically repair missing runner-up / Finals MVP history when the History page renders, when the playoff data is still available.

GitHub update:
Upload index.html and README.txt over the current files and commit.
Existing saves should continue working.
