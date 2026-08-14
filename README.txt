Basketballverse
v0.91.23 · IndexedDB Save Fix

ROOT CAUSE CONFIRMED
The screenshot shows:
"The quota has been exceeded."

Basketballverse was storing full universes in localStorage. Safari's localStorage
quota is too small for a multi-season universe.

NEW SAVE SYSTEM
- Full universes now save to IndexedDB instead of localStorage.
- IndexedDB has substantially more capacity and is designed for larger structured data.
- localStorage now keeps only the tiny Saved Universes index/metadata.

MIGRATION
- Existing localStorage saves are still readable.
- When an old save is opened, Basketballverse migrates it to IndexedDB.
- After a successful verified IndexedDB write, the large old localStorage copy
  is removed to free the quota.

VERIFICATION
- Every save is read back from IndexedDB before being marked successful.
- Save Now waits for the actual IndexedDB write to complete.
- Saved Universes uses the IndexedDB-aware loader.
- Load Existing Universe uses the same loader.

IMPORTANT
Progress made AFTER the last successful save in v0.91.22 exists only in the
currently open page memory. Reloading the page cannot recover that unsaved state.
Do not close the old tab if you still need something visible from that session.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
