Basketballverse
v0.91.10 · Clean Save Loader

IMPORTANT
This build intentionally starts from v0.91.5, before the v0.91.6-v0.91.9 save
button experiments. Those four versions layered multiple competing Play/load
systems on top of one another.

v0.91.10 has:
- one Saved Universes renderer
- one Play function
- one Load Existing Universe function
- one load path

PLAY / LOAD EXISTING
Both now call the exact same clean loader:
1. read localStorage using the game's original loadState()
2. restore the saved state
3. initialize missing old-save arrays
4. call the native showGame()
5. if showGame fails, display the exact runtime error in an alert and beneath
   Saved Universes

No query-string reloads.
No delegated Play handlers.
No pointer-capture hacks.
No overlay interception code.
No stacked replacement loaders.

All gameplay work through v0.91.5 is retained. The only removed code is the
unsuccessful v0.91.6-v0.91.9 saved-game experiments.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
