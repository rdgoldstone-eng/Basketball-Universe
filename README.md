# Basketballverse v0.91.47 — GM Career Profile

## What this build adds

This build turns the existing GM career data into a real career résumé for the person controlling the team.

### GM Career Profile
Open **Career → Profile** while playing as a GM to see:

- Championships won
- Playoff appearances
- Finals appearances
- Seasons as GM
- Career regular-season record
- Career winning percentage
- Number of franchises managed
- Best regular-season record
- Current GM reputation and job security
- A season-by-season GM résumé showing team, record, playoff appearance, and postseason result

The **Career History** submenu is relabeled **GM Résumé** in GM mode and shows the same tracked career results in a compact format.

### Historical/backfill behavior
- New completed GM seasons are snapshotted before Basketballverse starts the next season.
- Championships and Finals appearances come from the universe's permanent championship history.
- New playoff appearances are stored from the actual postseason field.
- For older saves created before this feature, Basketballverse reconstructs playoff appearances from archived franchise standings where possible. This is intended to preserve existing universes instead of forcing a restart.

## Version banner fix
The lower-right build banner is now controlled by the current build metadata and displays:

**Basketballverse v0.91.47 · GM Career Profile**

This patch also overrides the older hard-coded v0.91.43/v0.91.46 banner routines, which were why the footer could show an outdated version after newer builds were installed.

## Existing systems retained
This build is based on **v0.91.46 · Lottery Stability Fix** and retains:

- v0.91.45 Free Agency Economy changes
- Animated draft lottery
- Lottery fail-safe/escape behavior
- Historic newspaper headline logic
- Existing saves and universe history systems

## Installation / GitHub
Upload the contents of this folder to the same location currently hosting Basketballverse:

- `index.html`
- `basketballverse-logo.jpg`
- `README.md` (documentation only; the game does not need to load this file)

If GitHub Pages or your browser appears to show an older version after replacing `index.html`, verify the lower-right banner says **v0.91.47** and refresh the cached page.

## Test checklist
1. Load an existing GM universe.
2. Open **Career → Profile**.
3. Confirm past completed seasons appear in the résumé.
4. Confirm known championships are counted correctly.
5. Finish another season and advance to the next year.
6. Return to Career → Profile and confirm the new season was added once, with its playoff result.
7. Confirm the lower-right banner shows **v0.91.47 · GM Career Profile**.

## Build lineage
- v0.91.43 — Historic Newspapers
- v0.91.44 — Animated Draft Lottery
- v0.91.45 — Free Agency Economy
- v0.91.46 — Lottery Stability Fix
- **v0.91.47 — GM Career Profile**
