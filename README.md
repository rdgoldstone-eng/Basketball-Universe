# Basketballverse v0.96.39
## Permanent Draft Sim Control

The Draft Room's internal markup is still being redrawn by legacy renderer layers.
Instead of putting the simulation button inside that unstable section, v0.96.39
adds a permanent mobile-friendly control bar directly to document.body.

While the offseason is at Draft:
- Sim This Pick is always available
- Sim Rest of Draft is always available
- remaining picks are shown on the button
- once the draft completes, the same bar becomes Continue Offseason

Because this control lives outside the Draft Room renderer, it cannot disappear
when the old Draft Room UI redraws.

Player portraits in the Draft Room will be added after this control is confirmed working.
