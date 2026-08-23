# Basketballverse v0.95.09
## Universal Portrait Renderer Fix

**CURRENT BUILD: v0.95.09**

Built directly from v0.95.08.

All player displays now use the same portrait lookup:
- created/uploaded portrait
- registered historical portrait
- portraits/player_name.webp
- portraits/player_name.png
- portraits/player_name.jpg
- portraits/player_name.jpeg

Older roster/depth-chart/award/draft player cards are upgraded after render so they
also use the same portrait folder.

Test case:
`portraits/julius_erving.webp`

Load Philadelphia 76ers > Team > Roster. Julius Erving should show the image instead
of the JE fallback.
