# Basketballverse — v0.97.65

## Current Build

**v0.97.65 · Active Season Render Fix**

## Changes in v0.97.65

- Fixes the 1947–48 transition showing 1946–47 Season and Playoffs screens after the year has advanced. Reproduced the issue through the complete 1946 Commissioner season, playoffs, draft, and offseason on the deployed v0.97.64 build.
- The v0.97.63 and v0.97.64 refresh handlers checked `window.state`, but the game stores its active universe in a top-level `let state`; `window.state` is undefined. Those handlers returned without updating the screen. They now check the real game state before rendering the new season and clearing completed playoff panels.
- Updates the page banner, watermark, and build metadata to v0.97.65.

## Installation

Replace the repository-root `index.html` and `README.md` with the files in this folder. Keep your existing `portraits/`, `logos/`, and other asset folders. Existing browser saves stay in place.
