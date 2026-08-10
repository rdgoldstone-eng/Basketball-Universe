Basketball Universe
v0.82.14 · Chronicle & Draft History Persistence

FIXES
- Season-opening newspapers are permanently written into the Season > Seasons Chronicle archive.
- The newspaper is saved as soon as it is created, and again before Continue closes it.
- Missing newspaper editions can be rebuilt from completed season history.

- Draft History is now permanently saved during the draft, not only after the final post-draft render.
- Every completed pick updates the persistent draft-history entry.
- The final draft is archived before the game leaves Draft Room.
- Draft History refreshes immediately after saving.
- Missing draft-history entries from older broken builds can be reconstructed from offseason draft results or permanent player draft data.
- A stale/empty history object cannot overwrite a richer completed draft.

GOAL
If you can see a newspaper or a completed draft once, it should still exist later in its History screen and after reloading the save.

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root.
