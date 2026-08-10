Basketball Universe League
v0.83.1 · History UI & Recording Fix

WHAT WAS WRONG
There were two separate failures:
1. Awards/Draft results were not always being committed to permanent history at the moment they existed.
2. Open Awards / History navigation only switched screens and did not force History to render.

FIXES
- Awards results are committed directly to Season Honors + Champions during the Awards offseason stage.
- Draft results are committed directly from the completed offseason draft results.
- Open Full Awards History now explicitly writes the awards, opens History, and renders it.
- Opening History from navigation now renders History immediately.
- Opening Draft History now renders Draft History immediately.
- Added failure-resistant History rendering so one bad logo/record cannot blank the entire page.
- Added a simple direct Draft History renderer from the canonical stored draft results.
- Existing saves with offseason awardResults or draftResults are repaired on load.

TEST
1. Open Awards and tap Open Full Awards History.
2. Season Honors and Champions should show the completed season.
3. Open History > Draft History.
4. The completed draft should show if draftResults still exist in the save.

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root.
