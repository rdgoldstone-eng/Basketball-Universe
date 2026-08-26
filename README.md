# Basketballverse v0.97.00
## Stabilization Baseline

First cleanup/refactor build.

Removed the stacked Draft Room rescue layers introduced in v0.96.35-v0.96.39
and replaced them with one authoritative DraftControllerV09700.

Preserved:
- v0.96.34 playoff initialization fix
- historical data and draft classes
- save structure
- league/ABA/merger systems
- portraits and logo asset systems
- established draft-pick engine

Viewer Draft behavior now has one path for:
- draft initialization recovery
- loaded prospect visibility
- Sim This Pick
- Sim Rest of Draft
- draft completion
- Continue Offseason

No Draft Room redesign or portrait UI change is intentional in this build.
Next test: 1946 season -> 1947 playoffs -> offseason -> 1947 Draft -> next season.
