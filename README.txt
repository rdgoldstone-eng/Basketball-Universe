Basketballverse
v0.91.39 · Automatic Portrait Loader

BUG
The second portrait batch could be uploaded correctly but still not appear.
v0.91.36 only had explicit name mappings for Larry Bird, Magic Johnson, and
Michael Jordan.

FIX
Basketballverse now automatically looks for a portrait using the player's name:
portraits/charles-barkley.webp
portraits/hakeem-olajuwon.webp
portraits/patrick-ewing.webp
etc.

If the name-based file does not exist, it then tries the old player-ID filename.
If neither exists, the normal fallback portrait appears.

INCLUDED
This ZIP includes the full second portrait batch inside /portraits.

GITHUB
Upload:
- new index.html
- the entire portraits folder contents (or just the new WebP files if the folder already exists)

After this version, adding a portrait normally requires only adding:
portraits/first-last.webp
No new code mapping should be necessary.
