# Basketballverse — v0.97.53

## Current Build

**v0.97.53 · Reliable Webapp Updater**

## Changes in v0.97.53

- Fixes Update Now repeatedly reloading the cached build and returning to the same update notice.
- Requests an explicit cache-busted `index.html` instead of reloading the repository folder address.
- Verifies the published index version before leaving the current page.
- Shows when GitHub Pages is still publishing and safely retries before reloading.
- Corrects the update checker so the current build is v0.97.53 rather than the former hard-coded v0.97.50.
- Keeps saved universes intact because updating never clears browser storage.
- Preserves the safe historical draft repair from v0.97.52 and the Watch Game exit fix from v0.97.50.

## Installation

Replace the repository-root `index.html` and `README.md` with these files. Keep all existing `logos/`, `portraits/`, and other asset folders in place. Existing saved universes remain compatible.

For this first updater repair, open `index.html?bv=09753` once after GitHub Pages finishes deploying. From v0.97.53 forward, Update Now will verify and load the newly published index automatically.
