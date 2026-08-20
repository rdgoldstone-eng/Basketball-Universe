# Basketballverse v0.91.87 — Information Always Visible + Role Authority

## Permanent permission rule

**Information is visible to every role. Authority determines what can be changed.**

Menus are no longer greyed out merely because the current role lacks control.

Examples:
- Player can open Draft Room and follow the draft, but cannot make selections or draft-night trades.
- Player can view Free Agency, contracts, roster cuts and front-office information without signing/releasing players.
- Player can see the team's gameplan, rotation, player roles and development information without changing the Coach's choices.
- Viewer can inspect game information without management controls.

## Navigation
Old Player-mode menu blocking is overridden. Main and submenu buttons are kept enabled and clickable.

## View-only pages
Player mode now receives read-only versions of:
- Front Office
- Trade information
- Free Agency
- Re-signings/contracts
- Roster Cuts
- Draft Room
- Coaching/gameplan
- Rotation
- Player Roles
- Development

The information remains visible; role-specific action buttons are withheld.

## Permission framework
`roleCanEditV09187(area)` is the common authority check for future role work.

This is the model future Coach, GM, Owner, Commissioner and Viewer pages should follow.

## Version
v0.91.87 · Information Always Visible + Role Authority
