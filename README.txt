v0.68.3 Basketball Universe — Decision Loop Fix

BLOCKING FIX
- Injury decisions are now created once per actual injury episode.
- Resolving an injury decision will not recreate the same decision after the next simulated game while that player is still hurt.
- A later, separate injury can still create a new decision as intended.
- Older saves with an injury already in progress are assigned a stable injury episode ID automatically.

WHY THIS HAPPENED
v0.68.2 only checked whether an OPEN decision with the same title existed. As soon as you resolved it, the next game saw the same injured player and created the decision again.

TESTING NOTE
This build is intended as a blocker fix. Do not treat the current game as feature-complete yet; we are using normal GM play to identify anything that prevents a real season from flowing correctly.
