# Basketballverse v0.91.53 — Sequential Lottery Reveal + Tanking

## Draft Lottery Reveal
The clickable-tile lottery has been replaced.

The new presentation is intentionally simple:
- Open the Draft Lottery Reveal from Draft Order.
- Press **Reveal Next Pick**.
- The lottery order is revealed from the lowest lottery pick upward, ending at #1.
- Press **Reveal All** at any time to show the complete order.
- **Return to Draft Order** always exits the presentation.
- The reveal does not reroll the lottery. It displays the order Basketballverse already generated.

This removes the lottery machine, animation timing, and tile-click dependencies that were causing the previous presentations to fail.

## Stretch-run GM decision
At roughly 70 games, GM mode now has four choices:
1. Push for seeding
2. Protect health
3. Evaluate bench players
4. Prioritize draft position

### Prioritize draft position
This is the Basketballverse tanking option. The controlled team:
- rests veterans / prioritizes development conceptually,
- receives a meaningful late-season competitive penalty,
- can still win games — tanking does not force losses,
- records the strategy in league news.

The strategy affects only the remaining regular-season games after the decision.

### Other choices
- **Push for seeding** gives a small late-season competitive boost.
- **Evaluate bench players** carries a small competitive cost while representing developmental minutes.
- **Protect health** retains the existing health-oriented choice without deliberately weakening game results.

## Existing-save support
If a v0.91.52 or earlier save is currently sitting on an unresolved **Stretch-run priority** decision, the new tanking option is appended automatically.

## Previous work retained
- Free Agency cap display
- GM Career History Recovery
- GM playoff-objective fix
- Historical playoff formats
- Free-agency economy improvements
- Historically aware newspapers

## Version
**v0.91.53 · Sequential Lottery Reveal + Tanking**
