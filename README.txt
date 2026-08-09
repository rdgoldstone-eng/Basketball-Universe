v0.58.1 Basketball Universe — Mobile Create Fix

FIXED: CREATE UNIVERSE ON IPHONE / MOBILE SAFARI

LIKELY CAUSE
Basketball Universe contains a large embedded logo library.
Previous builds copied built-in logo data URIs into the saved universe.
Mobile Safari can have a much tighter localStorage quota than desktop browsers.

If localStorage rejected the save, JavaScript stopped before showGame(), making the Create Universe button appear to do nothing.

CHANGES
- Built-in logo image data is no longer duplicated inside browser saves.
- Historical/team logos are reconstructed from the artwork already embedded in index.html.
- User-uploaded custom logo artwork is preserved.
- Older saves that omit built-in artwork are rehydrated automatically.
- saveState() now catches browser-storage errors instead of crashing the game.
- Create Universe now opens the game even if persistence fails.
- A visible warning is shown if the browser cannot save locally.

NO VISUAL LOSS
This does not remove logos from the game.
It only removes redundant copies of built-in artwork from localStorage.

TEST
On iPhone:
1. Refresh/reopen Basketball Universe after GitHub Pages updates.
2. Choose Viewer.
3. Leave the start year at 1976.
4. Tap Create Universe.
5. The Dashboard should open immediately.
6. Refresh the page once afterward and use Load Existing Universe to confirm the save persisted.

GitHub update:
Upload index.html and README.txt over the current files and commit.
