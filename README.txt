Basketballverse
v0.91.26 · Trade Selection Ownership Fix

BUG
A draft pick was checked in the Trade Machine, then unchecked before submitting,
but the pick still transferred to the other team.

ROOT PROBLEM
The Trade Machine checkbox used a blind toggle:
- click = invert selected state

It did not send the checkbox's actual checked/unchecked value. With repeated
rerenders and accumulated trade wrappers, the visual checkbox and the internal
trade package could become out of sync.

FIX
- Checkboxes now explicitly send this.checked.
- checked=true guarantees the asset is selected.
- checked=false guarantees the asset is removed.
- Player/pick IDs compare safely as strings for older saves.
- Before submission, selected picks are validated against CURRENT ownership.
- Trade submission snapshots the exact final package.
- Draft-pick ownership is transactional:
  - rejected/failed trade = ownership restored
  - accepted trade = ONLY picks still selected in the final package transfer
- Old trade wrappers cannot transfer a pick that was removed before Submit.

NOTE
This prevents the bug going forward. A pick that was already incorrectly moved
in an older save cannot be safely guessed/reversed automatically because the
game cannot know whether that historical transfer was intended.

This build retains:
- IndexedDB saving
- Fired true Viewer mode
- Job Market acceptance
- Multi-asset Trade Finder
- projected draft-pick values
- traded-pick Draft Room ownership fix

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
