# Basketballverse v0.91.82 — Created Player Portrait Everywhere

## Uploaded image is now the player's actual portrait
A portrait uploaded on the Create a Player screen now feeds Basketballverse's global player portrait renderer.

That means the same uploaded image can appear wherever the game uses player portraits, including:
- roster/player cards
- player profiles
- Player Career
- career-person profile
- portrait-enabled league/history displays

## Save-size protection
The image remains stored once on the persistent Career Person rather than duplicating the same large data URI on both the person and player record.

The player record is marked as using the Career Person portrait, and the portrait renderer resolves it automatically.

## Persistent identity
The same image remains attached to the Career Person if the player later retires and becomes a Coach or GM.

## Career portrait changes
Uploading or clearing a portrait later from Career refreshes the controlled player's displayed image as well.

## Version
v0.91.82 · Created Player Portrait Everywhere
