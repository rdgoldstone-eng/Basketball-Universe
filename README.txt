Basketballverse
v0.91.9 · Startup Interaction Fix

WHAT WE LEARNED
The Saved Universes list itself is rendering, which proves Basketballverse's
JavaScript is loading. Since Play, Load Existing Universe, Create Universe and
other startup controls are all inert, this is broader than the saved-game loader.

THIS BUILD FIXES THE START SCREEN INPUT LAYER
- All startup buttons, links, selects and role cards are explicitly restored to
  pointer-events:auto and raised above accidental overlays.
- Known game overlays are forcibly cleared when the startup screen is visible.
- A hit-target repair checks whether another element is physically covering a control.
- A window-level pointer handler catches taps before a stray overlay can swallow them.
- Play and Load Existing Universe use the native saved-game URL launcher.
- Role selection, Rename and Delete also have startup-level fallback actions.

This is intentionally a start-screen interaction fix, not another saved-game
loader rewrite.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
