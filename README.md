# Basketballverse v0.95.08
## Single Portrait Folder System

**CURRENT BUILD: v0.95.08**

Built directly from v0.95.07.

## Permanent portrait setup

Basketballverse now uses one permanent root folder:

`portraits/`

You can add player pictures to GitHub one file at a time without rebuilding the game.

Example:

`Julius Erving` → `portraits/julius_erving.jpg`

Supported formats:
- WebP
- PNG
- JPG
- JPEG

The game automatically tries all four extensions.

Existing bundled historical portraits and created-player uploaded portraits still work and take priority.

See `PORTRAIT_FOLDER_INSTRUCTIONS.md` for the exact filename rules.

## Correct repository structure

Basketball-Universe/
- index.html
- README.md
- basketballverse-logo.jpg
- PORTRAIT_FOLDER_INSTRUCTIONS.md
- portraits/
  - julius_erving.webp
  - bill_walton.webp
  - etc.

Only image files should go inside `portraits/`.
