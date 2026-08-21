# Basketballverse v0.91.88 — Portrait Fallback Crash Fix
Fixes the `nextElementSibling.style` runtime crash caused by missing/broken player portraits.
Portrait fallbacks are now null-safe, so historical players without portrait images cannot interrupt depth-chart, awards, leaders, Hall of Fame, or other player-list rendering.
v0.91.87 role-authority behavior remains unchanged.
