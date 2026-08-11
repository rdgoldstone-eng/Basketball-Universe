Basketball Universe League
v0.88.7 · GM Readiness Init Fix

BUG
Fresh GM universes could throw:
TypeError: undefined is not an object
(evaluating 'state.gmReadiness.checks=checks')

CAUSE
The GM readiness checker could run before state.gmReadiness had been initialized.

FIX
- gmCoreChecksV088() now always initializes state.gmReadiness first.
- Fresh GM universes initialize readiness, objectives, and transaction storage
  before the first full render.
- Older saves are also repaired on load.

SAVE NOTE
Replacing index.html on GitHub Pages should not erase browser saves.
If the game says "Autosaved" in the header, browser saving is currently working.
Creating a brand-new universe each time intentionally starts from a new state;
you can continue the same saved GM universe across these code updates.

Upload index.html and README.txt to the GitHub Pages repository root.
