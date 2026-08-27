# Basketballverse v0.97.14
## Viewer Depth Chart Read-Only Fix

Two concrete fixes from the v0.97.13 test:

1. Viewer coaching information
v0.97.13 targeted the wrong visible containers. The actual Team -> Depth Chart
screen is populated from coachIdentityBox, coachGamePlanBox, coachRotationBox,
coachPlayerRolesBox and coachDevelopmentBox.

v0.97.14 writes the read-only Viewer information directly into those real boxes
after renderCoaching runs. Viewer can see team coaching identity, game plan,
rotation/minutes, roles & buy-in, development and depth chart, but cannot edit them.

2. Season advance crash
The screenshot showed:
TypeError: null is not an object (evaluating 'this.parentElement.textContent=...')

That came from image fallback handlers firing after their image row had already
been replaced. Those handlers now verify parentElement still exists before
writing initials.

No simulation rules or player data changed.
