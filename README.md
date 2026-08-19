# Basketballverse v0.91.84 — Player Career UI + Draft Flow Fix

## Career UI simplified
Player mode no longer has two stacked rows of Career submenus.

The only Career navigation row is:
- Player Career
- Profile
- Career History

The old Job Market tab is removed from Player mode because player contracts and movement belong inside Player Career.

Inside Player Career, the second submenu row (Overview / Business / Life & Relationships / Legacy) is removed.

The page now keeps the core overview visible and uses expandable sections for:
- Business & Contracts
- Life & Relationships
- Legacy & Records

This is designed specifically to reduce mobile clutter and excessive scrolling.

## Player draft fixed
Player mode no longer enters or controls Draft Room.

When the offseason reaches Draft, the Player sees:
**Let GM Handle Draft**

Selecting it:
- opens/initializes the draft internally
- lets every franchise AI make its selections
- includes the player's own franchise
- completes draft history normally
- handles undrafted players normally
- advances to the next offseason stage

The Player never goes on the clock and cannot get trapped waiting to make a pick.

## Draft routing cleanup
- Current Activity points Player mode back to Offseason during the draft.
- Direct Draft Room navigation is blocked for Player mode.
- Older auto-open Draft Room behavior is overridden for Player mode.

## Version
v0.91.84 · Player Career UI + Draft Flow Fix
