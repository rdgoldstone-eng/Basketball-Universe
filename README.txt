Basketball Universe League
v0.88.2 · Progress Feedback

PLAYTEST USABILITY FIX

The user reported that progression could feel like the button did nothing, causing repeated taps.

Changes:
- Long simulation actions now show a full-screen Working / Processing indicator BEFORE simulation begins.
- Mobile Safari gets a short render yield so the indicator is actually visible.
- While an action is processing, all buttons are temporarily locked.
- Repeated taps are ignored rather than starting the action again.
- The message changes to say the first tap is still processing.
- Regular-season sim intervals, playoff simulation, offseason progression, and draft simulation all use the processing state.
- Longer actions such as end regular season, finish playoff round, re-signings, free agency, and roster cuts specifically warn that they can take longer on a phone.
- The overlay disappears automatically when processing finishes or errors.

This does not change simulation results; it makes progression responsive and prevents accidental repeated actions.

Upload index.html and README.txt to the GitHub Pages repository root.
