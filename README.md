# Basketballverse — v0.97.39

## Current Build

**v0.97.39 · Natural Generated Player Names**

## Changes in v0.97.39

- Stops adding visible numbers such as `2` or `3` to duplicate generated-player names.
- Uses a much larger deterministic name pool to give duplicate fictional players a genuinely different natural name.
- Automatically repairs numbered fictional-player names in existing saves.
- Updates matching draft history, active draft results, season newspapers, awards, and news references when a generated player is renamed.
- Removes accidental numeric suffixes from historical players without changing their internal player IDs.
- Keeps duplicate players separate through their unique internal IDs rather than altering their display names.
- Does not rename, move, delete, or otherwise modify any portrait files.
- Preserves the two-edition newspaper cycle introduced in v0.97.38.
- Updates the home-page version and persistent watermark to v0.97.39.

## Existing Save Repair

Load the existing universe normally. The repair runs automatically after the save loads. A player such as `Corey Porter 2` will receive a natural replacement name, and references to that player in the draft newspaper and history will be updated.

## Test Checklist

- Load the saved universe containing `Corey Porter 2`.
- Return to the newspaper or draft history and confirm the numeric suffix is gone.
- Open the player's profile and confirm the same corrected name appears there.
- Continue into another draft and confirm generated prospects do not receive visible numeric suffixes.
- Confirm existing historical portraits still load with their current filenames.

## Repository Structure

```text
Basketball-Universe/
├── index.html
└── README.md
```

Keep the existing `logos/`, `portraits/`, and other asset folders in the GitHub repository. Replace only `index.html` and `README.md` with the files from this update.

## Save Compatibility

Existing browser saves remain compatible. Internal player IDs, careers, teams, statistics, contracts, and portrait files are preserved.
