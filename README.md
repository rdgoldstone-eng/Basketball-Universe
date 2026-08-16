# Basketballverse v0.91.54 — Direct Draft Reveal + Canadian Logos

## Draft lottery/reveal fix
The separate lottery overlay is no longer required.

The Draft Order page itself now contains the reveal system:
- **Reveal Pick #X** reveals the first-round order from the bottom upward.
- The reveal ends with the #1 pick.
- **Reveal All** immediately shows the full first-round order.
- **Reset Reveal** lets you replay the reveal.
- Reveal progress is stored in the universe save.
- Revealing picks does not reroll or alter the draft order.

This is intentionally plain HTML inside the existing Draft Order page so it does not depend on the previous modal, animation, tile, or timer systems.

## Toronto and Vancouver logos
Toronto Raptors and Vancouver Grizzlies expansion-era logos are now embedded directly inside Basketballverse rather than loaded from third-party image hosts. This prevents failed remote images from falling back to the generic team logo.

The Canadian expansion teams are refreshed on old saves as well, so an existing save that already created generic logo-library entries can rebuild those entries.

## Previous changes retained
- Stretch-run tanking / Prioritize Draft Position
- Free Agency cap display
- GM Career History Recovery
- GM playoff-objective fix
- Historical playoff formats
- Free-agency economy improvements
- Historic newspaper context

## Version
**v0.91.54 · Direct Draft Reveal + Canadian Logos**
