v0.68.1 Basketball Universe — Mobile Load Fix

Fixes v0.68 failing/hanging on phones.

Changes:
- Removed an accidental recursive start-year function that could lock the page.
- Changed the 3-logo library to lazy loading so the phone is not asked to render hundreds of logo images at once.
- Identities now show a lightweight list with a “View 3 Logos” button.
- Added Logo Library to League navigation.
- The Logo Library only renders when opened.
- Keeps the Early NBA / Growing NBA / Modern three-logo framework intact.

Use the same GitHub upload process: replace index.html and README.txt.
