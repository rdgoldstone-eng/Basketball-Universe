# Basketballverse — v0.97.41

## Current Build

**v0.97.41 · Mobile Draft + Update Recovery**

## Changes in v0.97.41

- Replaces the blocking **Sim Rest of Draft** loop with a mobile-safe, time-sliced simulation.
- Saves progress after small groups of picks so a stopped browser does not erase the entire draft.
- Removes the full-game `renderAll()` call from draft completion—the high-memory redraw associated with the white-screen failure.
- Advances a completed draft directly to Re-signings with a targeted offseason render.
- Removes defunct, inactive, folded, or missing teams from the remaining draft order before simulation.
- Prevents accumulated legacy draft buttons from running competing draft handlers.
- Adds a visible recovery panel when a screen or background operation throws an error.
- Adds **Recover Current Screen** and **Reload Basketballverse** recovery actions instead of leaving a blank page.
- Adds an automatic lightweight update check using the published README version.
- Adds a manual **Check for Update** button to the opening screen.
- Reloads newer builds with a versioned URL so iPhone/Safari does not keep reopening a stale `index.html`.
- Preserves the newspaper portraits from v0.97.40 and the natural generated-player names from v0.97.39.
- Updates the home-page version and persistent watermark to v0.97.41.

## Important First Update

Because older Basketballverse versions do not contain the new update checker, you may need to refresh Safari or reopen the web app once after publishing v0.97.41. After v0.97.41 is running, future versions can be detected and loaded through the new update system.

## Draft Recovery

If the existing save is still at the Draft stage, load it normally and select **Sim Rest of Draft** again. The new handler will repair the remaining draft order, simulate in small batches, preserve progress, and advance to Re-signings.

## Test Checklist

- Load the saved universe that previously failed five or six seasons into the timeline.
- Enter the Draft Room and confirm the v0.97.41 draft controls appear.
- Select Sim Rest of Draft and confirm its progress text updates while picks are made.
- Confirm the screen advances to Re-signings without turning white.
- Save, close, and reload the universe to verify the completed draft remains saved.
- On the opening screen, select Check for Update and confirm it reports v0.97.41 as current.

## Repository Structure

```text
Basketball-Universe/
├── index.html
└── README.md
```

Keep the existing `logos/`, `portraits/`, and other asset folders in the GitHub repository. Replace only `index.html` and `README.md` with the files from this update.

## Save Compatibility

Existing browser saves remain compatible. Draft progress, player records, historical data, portraits, and stored universes are preserved.
