# Basketballverse v0.97.05
## Viewer Personnel Sim Fix

The previous Viewer offseason bar depended on offseason.active / season.phase.
Those conditions can be false even while the UI is visibly sitting on
Re-signings, Free Agency, or Roster Cuts.

This build fixes those three stages directly.

Viewer mode now gets a guaranteed persistent button whenever the actual
offseason.phase is:
- Re-signings -> Sim Re-sign Players
- Free Agency -> Sim Free Agency
- Roster Cuts -> Sim Roster Cuts

These buttons call the existing league AI functions directly, mark that stage
processed, advance exactly one offseason phase, save, and re-render.

Draft simulation remains unchanged.
