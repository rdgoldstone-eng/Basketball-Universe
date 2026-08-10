Basketball Universe League
v0.83 · History Ledger Rebuild

OFFICIAL NAME
The game is now named BASKETBALL UNIVERSE LEAGUE.
Internal browser-storage keys remain unchanged so existing saves stay compatible.

WHY THIS BUILD
The issue is larger than Newspaper or Draft History individually:
the game was not maintaining one reliable source of truth for league history.

NEW CANONICAL HISTORY LEDGER
- Seasons / awards
- Champions / runners-up / Finals MVP
- All-Star history
- League records
- Draft history
- Newspaper archive

The ledger is:
- initialized on every universe
- updated at actual season and draft milestones
- saved independently from the main universe save
- merged back when a save loads
- rebuilt from surviving player/season/draft data where possible

MILESTONE WRITES
- Season Complete immediately snapshots awards + champion into history.
- Draft completion immediately snapshots the full draft.
- Newspaper archive is rebuilt from the completed season and following draft.
- Start Next Season writes the outgoing season BEFORE offseason/draft state resets.

EXISTING SAVE REPAIR
Opening History or Draft History now triggers a full history rebuild from any
surviving universe data. If the old broken builds never stored enough source
information, some old details may be unrecoverable; future seasons will use
the new ledger automatically.

INSTALL
Upload index.html and README.txt to the GitHub Pages repository root.
