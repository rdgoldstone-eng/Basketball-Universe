v0.37.5 Basketball Universe — Rookie Simulation Fix

FIXED: ADVANCE BUTTON APPEARING TO STOP AFTER OFFSEASON

Root cause:
- The original 1976 players include historical per-36 stat data.
- Newly drafted players do not.
- Once a drafted rookie entered a rotation, the regular-season simulator tried to read missing historical data and the first game crashed silently.

Fix:
- Added a universal player per-36 profile.
- Historical players still use their supplied historical context.
- Drafted, generated, and custom players now derive scoring/rebounding/assists/steals/blocks from their ratings when historical data is unavailable.
- New players automatically receive initialized season-stat totals before playing.
- The same fallback is used by regular-season box-score generation.

This is important beyond the bug fix: alternate-history players no longer depend on real-life NBA statistics to function after being drafted.

Your existing save should continue working. You do not need to restart.

GitHub update:
Upload index.html and README.txt over the current files and commit.
