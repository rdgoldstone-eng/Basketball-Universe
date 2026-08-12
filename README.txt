Basketballverse
v0.91.8 · Saved Game Native Link Fix

WHAT CHANGED
The Saved Universes Play control is no longer dependent on a JavaScript click
listener. It is now a real browser link.

Tapping Play:
1. navigates to the same Basketballverse page with the save ID in the URL,
2. reloads the page normally,
3. reads that save directly from browser storage,
4. restores it,
5. opens the game screen.

This is intentionally different from v0.91.6 and v0.91.7. Those builds kept
trying to repair the same click-handler approach. This build removes that
approach from the critical Play path.

DIAGNOSTICS
If the save still cannot open, the start screen will now show the actual reason:
- stored save data missing
- browser storage unavailable
- save data could not be restored
- game screen failed while opening

Existing saves are not deleted or recreated.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
