# Basketballverse v0.96.33
## 1946-47 Playoff Entry Root Fix

The actual failure was in the v0.96.31 historical-bracket initializer itself:
it refused to initialize unless `state.currentYear === 1946`.

The UI/end-of-season state can expose a different current calendar year while
`state.season.year` still correctly identifies the 1946-47 season. That meant
v0.96.32 successfully caught the button click, called the new initializer, and
the initializer immediately returned false — visually making the button appear
to do nothing.

v0.96.33:
- identifies the inaugural season from `state.season.year`
- creates the six-team 1947 BAA bracket directly
- no longer depends on the faulty v0.96.31 currentYear guard
- directly intercepts OPEN PLAYOFFS and BEGIN PLAYOFFS
- switches to the Playoffs tab after successful creation
- keeps the historically correct 1947 postseason structure
- does not require a new save
