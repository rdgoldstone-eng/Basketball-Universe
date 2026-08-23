# Basketballverse v0.95.10
## Direct Roster Portrait Fix

**CURRENT BUILD: v0.95.10**

Built directly from v0.95.09.

## Root cause found

Team > Roster is ultimately rebuilt by the old v0.91.41 `cleanPlayerCardHTMLV09140`
renderer. That later renderer was overriding/bypassing the previous portrait fixes.

v0.95.10 directly replaces the final roster-card renderer and final roster rebuild
function.

It also resolves portrait URLs against `document.baseURI` and adds a version query
string to prevent a browser/GitHub Pages cached 404 from hiding a newly uploaded image.

## Exact test

Keep this file in GitHub:

`portraits/julius_erving.webp`

Then load:
Team > Roster > Philadelphia 76ers

Julius Erving should show that image in place of the JE silhouette.

No portrait folder or filename changes are required.
