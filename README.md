# Basketballverse v0.97.12
## Rotation Actually Moved to Depth Chart

v0.97.11 fixed the player-profile modal correctly, but its Rotation relocation
targeted the wrong DOM container.

v0.97.12 fixes the actual Team UI structure:
- The canonical existing #rotationCard is physically moved out of the Players /
  Roster section.
- It is appended to the actual Team -> Depth Chart section.
- CSS guarantees #rotationCard cannot display while it is under #players.
- Duplicate Rotation cards recreated in the Roster section are removed.
- The working v0.97.11 player-profile pop-up is unchanged.

No rotation calculations, minutes, depth-chart logic, player data, or simulation
logic changed.
