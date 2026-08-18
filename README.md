# Basketballverse v0.91.67 — Safari Syntax Compatibility Fix

## Critical fix
Recent Coach builds introduced a few JavaScript expressions that mixed `??` with `||` without parentheses. Safari/iPhone refuses to parse JavaScript containing that syntax, which caused the startup “Unexpected token '||'” Game error.

This build corrects those expressions.

## Verification
Every inline JavaScript block in `index.html` was checked with a JavaScript parser before packaging this build. The build passed with zero syntax errors.

## Preserved work
All features through v0.91.66 remain included:
- Coach Hall of Fame and Greatest Coaches
- Coach jobs, contracts, firing, and career movement
- Coach → GM progression
- Persistent Career Person
- Character portrait foundation
- Opponent scouting and halftime adjustments
- Interactive crunch time
- Editable Coach depth chart
- Coach career, legacy, attributes, and awards
- Earlier GM, offseason, free-agency, playoff, and history fixes

## Version
v0.91.67 · Safari Syntax Compatibility Fix
