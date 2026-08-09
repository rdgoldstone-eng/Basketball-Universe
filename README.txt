v0.67.1 Basketball Universe — Logo Coverage Fix

This is a quick logo-coverage repair build for the 2026 Current Day universe.

FIXES
- Added missing current-team logo coverage for all 30 active NBA franchises.
- Specifically repairs the Clippers, Kings and Wizards in the current-day snapshot.
- Added a broader current-team fallback library so Charlotte, Miami, Orlando, Minnesota, Toronto and other modern teams no longer drop to default initials when their older embedded logo coverage is missing.
- Updated the logo browser so these count as covered assets instead of generic fallbacks.

HOW IT WORKS
- Historical embedded logos still load first when available.
- If a modern current-team logo is missing from the older embedded asset set, the game now falls back to an official current-team remote logo source.
- The white logo-card background is preserved for visual consistency.

NOTE
This is a coverage fix, not the final full historical PNG pass. If this works well, the next logo pass can replace more of these modern fallbacks with fully embedded white-background PNG assets.
