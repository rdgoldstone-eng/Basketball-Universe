# Basketballverse v0.91.55 — Local Canadian Logo Asset Fix

## Toronto & Vancouver
The previous fix still allowed Toronto and Vancouver to pass through the generic logo-library path.

This version includes two local logo assets:
- `logos/toronto-raptors-1995.svg`
- `logos/vancouver-grizzlies-1995.svg`

The game now hard-routes Toronto Raptors and Vancouver Grizzlies to those local files before any generated or remote logo fallback can run.

Existing saves are also repaired by clearing cached generic logo entries for those teams.

## Important
Upload the **entire ZIP contents**, including the `/logos` folder, to GitHub. If only `index.html` is uploaded, the two local logo files will not be available.

## Other features retained
- Direct Draft Order reveal
- Stretch-run tanking
- Free Agency cap display
- GM Career History Recovery
- Historical playoff formats
- Free-agency economy improvements
- Historically aware newspapers

## Version
**v0.91.55 · Local Canadian Logo Asset Fix**
