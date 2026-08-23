# Basketballverse Portrait Folder

Use ONE folder only:

`/portraits/`

Upload individual player image files directly into that folder.

## Filename rule

Use the player's name in lowercase with spaces changed to underscores.

Examples:

- Julius Erving → `julius_erving.jpg`
- Bill Walton → `bill_walton.png`
- Pete Maravich → `pete_maravich.webp`
- Bernard King → `bernard_king.jpeg`
- Kareem Abdul-Jabbar → `kareem_abdul_jabbar.jpg`

Apostrophes and punctuation are removed:
- Shaquille O'Neal → `shaquille_oneal.jpg`

## Supported formats

The game automatically tries:

1. `.webp`
2. `.png`
3. `.jpg`
4. `.jpeg`

You do NOT need to edit `index.html` when adding a portrait.

You do NOT need to rebuild Basketballverse when adding a portrait.

Do not place README files, index.html, logos, ZIP files, or other game files inside `/portraits/`.

The repository root should contain `index.html`, README files, the Basketballverse logo, etc.
Only player-image files belong inside `/portraits/`.
