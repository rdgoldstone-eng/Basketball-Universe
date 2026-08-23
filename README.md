# Basketballverse v0.92.02 — Owner Draft Button Fix

Built directly from v0.92.01.

## Exact bug fixed
The Draft Room already recognized the Indiana Pacers as the controlled team and displayed:
- Indiana Pacers is on the clock
- YOUR PICK
- Draft buttons

However, pressing Draft called the older `gmDraftPlayerV0881()` handler. That handler required `isHumanGMV084()`, which returns true only for GM mode. Therefore Owner mode displayed the correct pick but rejected the button press with:
`Your team is not currently on the clock.`

v0.92.02 removes that obsolete GM-only requirement. The Draft button now uses the game's real `isUserDraftPick()` check, which already supports both GM and Owner.

## Package
- index.html
- README.md
- basketballverse-logo.jpg
- historical Raptors and Grizzlies logo assets

All Owner systems from the previous builds remain included.


## v0.92.03 — Owner Re-Signings Advance Fix
- Owner mode can review Re-Signings but does not negotiate player contracts directly.
- Adds a clear **Let GM Handle Re-Signings & Continue** button during the Re-Signings stage.
- Uses available AI/GM re-signing logic when present.
- Advances the offseason through the normal engine, temporarily delegating authority only for that transition.
- Restores Owner role immediately afterward.


## v0.92.04 — Owner Free Agency Advance Fix
- Owner mode can view the entire Free Agency stage.
- Adds **Let GM Handle Free Agency & Continue**.
- Uses available AI/free-agency completion logic where present.
- Delegates only the authority needed to move the offseason forward.
- Restores Owner role immediately afterward.


## v0.92.05 — Owner Roster Cuts Advance Fix
- Owner mode can review the roster-cut stage.
- Adds **Let GM Handle Roster Cuts & Continue**.
- Uses available AI/GM roster-cut logic where present.
- Delegates only the authority needed to advance the offseason.
- Restores Owner mode immediately afterward.


## v0.92.06 — Owner Trade Requests + Attendance + City Pitches

### Owner trade targets
Career → Decisions now includes an Owner-only section to ask the GM to pursue a specific player.
- Owner selects a target.
- GM responds after a short delay.
- Accepted requests become real front-office trade targets.
- Owner does not negotiate or execute the trade.

### Attendance
Owner Career now tracks:
- Average Attendance
- Capacity Filled
- Attendance Grade (A+ through F)
- Attendance Trend (Rising / Stable / Falling)

Attendance responds to:
- team performance
- fan support
- market strength
- arena quality
- ticket prices

Attendance is stored in ownership data and season history.

### Cities approach ownership
Outside cities can now approach the Owner about moving the franchise when:
- attendance is weak or falling
- market strength is poor
- arena pressure is high
- relocation pressure is elevated

Owner can:
- Hear the Proposal
- Use the offer as leverage
- Reject the approach

Hearing a proposal can place the franchise/city into the relocation-candidate framework without automatically moving the team.
