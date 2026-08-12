Basketballverse
v0.90.5 · Header Rename Fix

FIX
The top game logo/banner was built as separate elements:
BASKETBALL
UNIVERSE

That is why earlier replacements of the phrase "Basketball Universe" did not
change the visible header.

This build explicitly handles the split header markup and changes it to:
BASKETBALLVERSE

The document title and dynamic rerenders are also corrected.

Legacy internal save keys remain unchanged for compatibility.
