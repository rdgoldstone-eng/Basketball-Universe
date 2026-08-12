Basketballverse
v0.91.6 · Saved Game Play Fix

FIX
- Rebuilt the saved-game Play action so dynamically rendered Play buttons always work.
- Added a repair pass for older saves before opening them.
- Missing/invalid controlled-team references are repaired when possible.
- Missing arrays/history/offseason fields from older versions are initialized safely.
- The game screen now opens even if a secondary page-render function throws an error.
- If a specific screen fails after load, Basketballverse reports that error instead of making the Play button look dead.
- Loaded saves open at their current simulation stage (season/playoffs/offseason/draft) when possible.

This does NOT delete or recreate the user's existing save.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
