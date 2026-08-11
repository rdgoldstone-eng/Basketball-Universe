Basketball Universe League
v0.88.3 · Safe Progress Feedback

WHY THIS REPLACES v0.88.2
v0.88.2 wrapped core simulation functions. On the user's phone that introduced
runtime "Can't find variable" errors.

v0.88.3 starts again from the known-working v0.88.1 code and adds feedback WITHOUT
replacing or rerouting the simulation engine.

CHANGES
- Progress message appears immediately when a long simulation/progression button is tapped.
- Original button onclick/function remains untouched.
- Repeated taps are blocked while the first tap is processing.
- The feedback message stays on screen while synchronous work blocks the browser.
- It clears when the game renders the updated state.
- Runtime errors now show the actual browser error message instead of the vague
  "Action stopped" message.

IMPORTANT
This build intentionally discards the v0.88.2 wrapper implementation while keeping
the v0.88.1 GM draft-selection and trade-feedback fixes.

Upload index.html and README.txt to the GitHub Pages repository root.
