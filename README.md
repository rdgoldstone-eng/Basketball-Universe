# Basketballverse v0.97.04
## Complete Viewer Offseason Sim Controls

Built from the confirmed-loading v0.97.03 build.

This pass specifically checks and guarantees Viewer simulation controls for:
- Re-sign Players
- Free Agency
- Roster Cuts

The controls recognize small differences in the game's historical phase labels
(e.g. Re-signings vs Re-Sign Players) instead of relying on one exact string.

They reuse the existing v0.97.03 persistent offseason control bar and the game's
existing offseason advance engine, so no second competing offseason UI is added.

The working Draft simulation controls remain unchanged.
