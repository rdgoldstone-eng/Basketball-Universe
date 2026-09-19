# Basketballverse — v0.97.56

## Current Build

**v0.97.56 · Startup Freeze Repair**

## Changes in v0.97.56

- Fixes the setup screen freezing partway through its second section on mobile Safari.
- Removes the competing whole-page version observer introduced in v0.97.54/v0.97.55.
- Updates the game's original stable-version controller directly to v0.97.56 so only one observer owns the banners.
- Keeps the setup banner, bottom watermark, update checker, runtime build identity, and static metadata synchronized.
- Retains the CSS-backed version display without creating a JavaScript observer loop.
- Preserves the reliable updater, safe historical draft repair, and Watch Game exit fix.

## Installation

Replace the repository-root `index.html` and `README.md` with these files. Keep all existing `logos/`, `portraits/`, and other asset folders in place. Existing saved universes remain compatible.

Use Update Now after GitHub Pages finishes deploying. The updater verifies the published `index.html` before loading it.
