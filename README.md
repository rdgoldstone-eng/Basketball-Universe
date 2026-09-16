# Basketballverse — v0.97.55

## Current Build

**v0.97.55 · Locked Version Identity**

## Changes in v0.97.55

- Replaces the original hard-coded v0.97.26 setup label in the page source.
- Locks the visible setup banner and bottom watermark to v0.97.55 at the CSS level, so older scripts cannot visually repaint them.
- Keeps the static metadata, updater comparison, runtime build identity, setup banner, and watermark synchronized.
- Retains the render and page-restoration safeguards from v0.97.54.
- Preserves the reliable updater, safe historical draft repair, and Watch Game exit fix.

## Installation

Replace the repository-root `index.html` and `README.md` with these files. Keep all existing `logos/`, `portraits/`, and other asset folders in place. Existing saved universes remain compatible.

Use Update Now after GitHub Pages finishes deploying. The updater verifies the published `index.html` before loading it.
