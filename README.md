# Basketballverse — v0.97.59

## Current Build

**v0.97.59 · Unique Draft Prospects**

## Changes in v0.97.59

- Removes duplicate people when historical draft sources are combined. The 1947 draft board now lists Carl Braun once instead of adding “Carl Braun 2.”
- Checks an active draft before each pick, including picks loaded from an existing save, so a prospect already selected cannot be selected again under another entry.
- If the latest pick in an active draft duplicated an earlier pick and the matching rookie is still identifiable, restores that team's pick and removes the duplicate rookie. Earlier completed drafts are not rewritten automatically.
- Preserves the commissioner league events and offseason presentation from v0.97.58.

## Installation

Replace the repository-root `index.html` and `README.md` with the two files in this ZIP. Keep your existing `portraits/`, `logos/`, and other asset folders. Saved universes remain in the browser.

If a duplicated pick is the most recent pick in an active draft, reopen the Draft Room to select another player. If the draft has already advanced past that pick, the prior pick is retained so that later draft history and rosters are not silently changed.
