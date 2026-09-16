# Basketballverse — v0.97.54

## Current Build

**v0.97.54 · Authoritative Version Banners**

## Changes in v0.97.54

- Makes v0.97.54 the authoritative version for the setup banner, fixed bottom watermark, update checker, and static build metadata.
- Stops older render routines from repainting the visible version labels as v0.97.50.
- Reapplies the current label after full game renders, page restoration, and returning to the browser tab.
- Watches the two visible labels and immediately corrects them if an older routine changes their text.
- Preserves the reliable cache-busted updater from v0.97.53.
- Preserves the safe historical draft repair and Watch Game exit fix.

## Installation

Replace the repository-root `index.html` and `README.md` with these files. Keep all existing `logos/`, `portraits/`, and other asset folders in place. Existing saved universes remain compatible.

Use Update Now after GitHub Pages finishes deploying. The updater verifies the published `index.html` before loading it.
