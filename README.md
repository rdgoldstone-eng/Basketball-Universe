# Basketballverse v0.96.38
## Stable Draft Simulation Buttons

Built directly from v0.96.37 after seeing the flashing button on iPhone.

Root cause:
v0.96.37 used a 250 ms DOM watchdog to keep the loaded draft prospects visible.
That watchdog continuously destroyed and recreated the Sim Draft buttons. On a
touch device, a button could disappear between touch-down and touch-up, so it
looked like it flashed but the click never completed.

v0.96.38:
- removes the 250 ms Draft Room DOM replacement loop
- keeps the visible Draft Room stable
- binds Sim This Pick and Sim Rest of Draft with persistent click handlers
- prevents click propagation from triggering unrelated redraws
- re-renders only after the draft action finishes
- retains the loaded 1947 prospects and draft order

Player portraits in the Draft Room are the next UI addition once the simulation
buttons are confirmed working.
