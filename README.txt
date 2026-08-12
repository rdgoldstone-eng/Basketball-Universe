Basketballverse
v0.91.4 · Trade, Age & Layout Fix

LAYOUT
- Removed the old static Offseason HTML that contained leftover Draft Results and Free Agency cards.
- Free Agency no longer appears underneath unrelated screens such as Trade Machine.
- The main Offseason page remains the compact checklist + selected-task box from v0.91.1/v0.91.2.

TRADE MACHINE
- Fixed malformed / missing draft-pick data causing:
  undefined is not an object (evaluating 'pk.round')
- Missing draft-pick records are ignored rather than crashing the page.
- Stale player/pick IDs in an old saved trade builder are cleaned automatically.
- If a save contains a bad selected pick, the Trade Machine retries with those bad pick selections cleared.

PLAYER AGES
- Added stable season-age tracking using a birthYear anchor.
- Existing players get a birthYear derived from their current saved age.
- Ages are synchronized to the current season after load/render so they cannot be lost or double-aged by repeated offseason operations.
- Free Agency and Roster Cuts now explicitly show player age alongside position/OVR/contract information.
- Existing player pages and rosters continue showing age as before.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
