# Basketballverse — v0.97.43

## Current Build

**v0.97.43 · Version Lock + Cache Refresh**

## Changes in v0.97.43

- Fixes the older stable-version safeguard that was still locked to v0.97.41.
- Synchronizes every active version label in the file to v0.97.43.
- Keeps the opening-screen banner and persistent watermark on the current version after game renders, saved-universe loads, and tab changes.
- Adds a unique timestamp to **Update Now** reload URLs so iPhone and Safari cannot reuse the same cached update address.
- Preserves the v0.97.42 malformed-name repair, historical portrait-key recovery, newspaper portrait resolution, and forced post-draft transition to Re-signings.

## Why v0.97.42 Displayed v0.97.41

The v0.97.42 file was published correctly, but an older version-protection block still treated v0.97.41 as the permanent display version. It continuously changed the visible banner and watermark back to v0.97.41. This update corrects that block at its source.

## Updating from v0.97.42

Replace `index.html` first and then replace `README.md`. After GitHub Pages finishes publishing, the existing **Update Now** button should detect v0.97.43. Its first reload still uses the older update method; if the home-screen app remains on v0.97.41, close it completely and reopen it once. Future updates use the strengthened cache-refresh address.

## Test Checklist

- Confirm the opening-screen banner shows v0.97.43.
- Load an existing universe and confirm the persistent watermark remains v0.97.43.
- Change tabs and simulate an event; confirm neither version label returns to v0.97.41.
- Confirm the repaired player names and newspaper portraits from v0.97.42 remain intact.
- Finish a draft and confirm the offseason advances to Re-signings.

## Repository Structure

```text
Basketball-Universe/
├── index.html
└── README.md
```

Keep the existing `logos/`, `portraits/`, and other asset folders. Replace only `index.html` and `README.md` with the files from this update.

## Save Compatibility

Existing browser saves remain compatible. This update changes version-display and reload behavior without deleting or resetting saved universes.
