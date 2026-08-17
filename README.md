# Basketballverse v0.91.57 — Coach Offseason Authority Fix

## Coach re-signing loop fixed
Coach mode was reaching the league Re-signings stage, but the offseason UI still directed the user into Front Office contract controls. That created a loop because those decisions belong to the GM.

Coach mode now has explicit role authority during the offseason:

- **Re-signings:** `Let GM Handle Re-signings`
- **Free Agency:** `Let GM Handle Free Agency`
- **Roster Cuts:** `Let GM Finalize Roster`

The AI front office handles those personnel stages for the Coach's team and every other team, then the offseason advances normally.

Coach mode no longer needs to open Front Office or manually sign/release players to continue.

## Existing save repair
A Coach save already stuck on Re-signings, Free Agency, or Roster Cuts will reopen on the Offseason page with the correct action available.

## Coach role retained
v0.91.56 Coach Career, expectations, résumé, rotations, schemes, development focus, roles/buy-in and coaching systems remain intact.

## Version
v0.91.57 · Coach Offseason Authority Fix
