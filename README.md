# Basketballverse — v0.97.44

## Current Build

**v0.97.44 · Always-Available Draft Simulation**

## Changes in v0.97.44

- Refreshes the Draft simulation controls whenever the Draft Room or offseason screen renders.
- Refreshes the controls after navigation, so entering the Draft later in a session no longer leaves the simulation bar hidden.
- Adds an **Open and Sim Draft** recovery action when the Draft stage exists but the Draft Room has not initialized.
- Repairs and initializes the Draft Room before attempting to simulate an incomplete draft.
- Gives Viewer and Commissioner modes **Sim This Pick** and **Sim Rest of Draft** controls.
- Gives controlled roles **Sim This Pick**, **Sim to My Pick**, and **Sim Rest of Draft** controls.
- Allows **Sim Rest of Draft** to simulate controlled-team selections instead of stopping when the user's team comes on the clock.
- Keeps the mobile simulation time-sliced so long drafts do not lock the screen.
- Preserves the forced transition to Re-signings after the draft finishes.
- Synchronizes the opening banner, persistent watermark, README, and update checker to v0.97.44.
- Preserves all v0.97.42 player-name and newspaper-portrait repairs and the v0.97.43 version-lock/cache correction.

## Test the Existing Draft Save

Load the universe that is currently at the Draft stage. The bottom Draft control bar should appear automatically.

- If the Draft Room was not initialized, select **Open and Sim Draft**.
- To simulate only the current selection, select **Sim This Pick**.
- In a controlled role, **Sim to My Pick** stops when your team is on the clock.
- **Sim Rest of Draft** completes every remaining selection, including selections belonging to the controlled team.
- When the draft finishes, Basketballverse advances to Re-signings.

## Repository Structure

```text
Basketball-Universe/
├── index.html
└── README.md
```

Keep the existing `logos/`, `portraits/`, and other asset folders. Replace only `index.html` and `README.md` with the files from this update.

## Save Compatibility

Existing browser saves and partially completed drafts remain compatible. The update repairs the active Draft Room without discarding completed selections.
