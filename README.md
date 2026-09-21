# Basketballverse — v0.97.73

## Current Build

**v0.97.73 · 1967 Era Start Repair**

## Changes in v0.97.73

- Fixes an endless recursive call when changing the Starting Era. Selecting 1967 now finishes the setup update instead of stopping before the team choices and Create Universe button can work.
- Fixes the 1967 NBA/ABA selector repeatedly rewriting the team list. The options only change when switching leagues. Removes the document-wide mutation observer; the selector responds to the Starting Era and League controls directly.
- Corrects setup copy that described the already installed 1946 and 1967 snapshots as future work.
- Preserves the v0.97.72 relocation form, uploaded logos, and existing saved universes. Updates the build banner, watermark, and metadata.

## Verification

The JavaScript passed syntax checks. Targeted checks verified that changing eras completes without recursion, repeated NBA/ABA selector updates stabilize, and the 1967 Commissioner creation path accepts the included 12-team NBA opening snapshot and ABA rival-league data. A full browser playthrough remains to be checked during your test.

## Installation

Replace the repository-root `index.html` and `README.md` with these files. Keep the existing `portraits/`, `logos/`, and other asset folders. Your browser saves stay in place.
