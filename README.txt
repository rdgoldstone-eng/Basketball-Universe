Basketball Universe League
v0.88.5 · Stable Trade Machine Subtab

FIX
The previous v0.88.4 Trade Machine subtab used a second custom navigation/page system.
That was unnecessary and could trigger a ReferenceError.

This version starts from the known-working v0.88.3 build and adds Trade Machine
directly to the game's existing Front Office navigation group.

Front Office subtabs:
- Scouting
- Draft Room
- Front Office
- Trade Machine
- Ownership

The Trade Machine is a normal .section just like every other game tab.
No dynamic page creation. No replacement navigation engine.

The existing GM trade builder and accepted/rejected feedback from v0.88.1 are retained.
The safe progress feedback from v0.88.3 is retained.

Upload index.html and README.txt to the GitHub Pages repository root.
