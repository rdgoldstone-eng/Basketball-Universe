# Basketballverse v0.93.13
## Global Decisions Center

**CURRENT BUILD: v0.93.13**

Built through the full first Commissioner development pass.

## Commissioner systems now included
- Commissioner career metrics and persistent decisions
- League Office
- Franchise risk / Stable-Monitor-Watch-Critical oversight
- Owner relationship tracking
- Arena, financial and relocation interventions
- Relocation and rebrand approval queue
- Expansion Office with city bids, finalists and franchise awards
- Board of Governors rule proposals and owner voting
- League media-package strategy
- Revenue-sharing policy
- Dynamic discipline/dispute cases
- Commissioner Career & Legacy score/history
- League-wide attendance and franchise-health monitoring

## Testing target
This is the first Commissioner build intended for an actual play-through test. The goal is to test whether Commissioner has enough meaningful work without directly controlling team basketball operations.

Package includes index.html, README.md, Basketballverse logo, and historical Raptors/Grizzlies assets.


## v0.93.07 — Commissioner Re-Signings Advance Fix
- Adds **Let Teams Handle Re-Signings & Continue**.
- Commissioner can review re-signings without negotiating team contracts.
- Team AI/front offices handle the stage.
- Commissioner role is restored immediately after advancing.


## v0.93.08 — Commissioner Free Agency + Roster Cuts Advance Fix

### Free Agency
- Adds **Let Teams Handle Free Agency & Continue**
- Commissioner can review league-wide free agency without controlling team signings
- Team AI/front offices handle the stage

### Roster Cuts
- Adds **Let Teams Handle Roster Cuts & Continue**
- Commissioner can review roster compliance and cuts without controlling team releases
- Team AI/front offices handle the stage

### Offseason role behavior
Re-Signings, Free Agency, and Roster Cuts now all have Commissioner-safe delegation paths so the role cannot get trapped in team-controlled offseason stages.


## v0.93.09 — Commissioner Direct Offseason Simulation
Commissioner no longer needs to open team-operation pages for:
- Re-Signings
- Free Agency
- Roster Cuts

Current offseason actions are replaced with:
- **Simulate Re-Signings**
- **Simulate Free Agency**
- **Simulate Roster Cuts**

Each button lets team AI/front offices handle the entire phase and advances the offseason directly.

Older Commissioner delegation boxes from v0.93.07/v0.93.08 are removed from the offseason screen.

## v0.93.10 — Global Decisions Center
- Decisions is now a permanent top-level main menu item, not buried under Career.
- A gold count badge shows unresolved decisions from anywhere in the game.
- Decisions is removed from Career subnavigation.
- Player, Coach, GM, Owner, and Commissioner all have role-specific decision inbox support.
- Pending Player season/offseason decisions, Owner decisions/city approaches, Commissioner decisions/approvals/cases, and existing Coach/GM career decisions are collected here.
- Decision history is shown on the same page.
- Unresolved decisions remain visible until answered.


## v0.93.11 — Decisions Navigation Fix
- Simulation no longer automatically jumps to the Decisions screen.
- New decisions still remain in the Decision Center.
- The Decisions main-menu badge still updates and highlights when something is waiting.
- Players can continue simulating and open Decisions when they choose.


## v0.93.12 — Expansion + Relocation Logo Previews
- Expansion city bids now show a proposed team identity and logo preview.
- Commissioner relocation approval cards now show the proposed destination identity/logo.
- Owner city relocation approaches use the same visual identity preview.
- If a matching team/logo already exists in the universe, Basketballverse reuses the existing logo.
- If no finalized logo exists yet, the preview uses a clean city/team abbreviation placeholder until the identity is finalized.


## v0.93.13 — Franchise Decisions + Identity Preview
- The actual **Add Expansion Franchise** controls now show a large preview for the currently selected team identity.
- The actual **Relocation** controls now show the proposed destination identity/logo before approval.
- Changing the market or identity immediately refreshes the preview.
- Expansion and relocation are now also surfaced in the Commissioner's **Decisions** area as major franchise decisions.
- The existing League Office controls remain the detailed management screen; Decisions is the prominent decision/inbox entry point.
