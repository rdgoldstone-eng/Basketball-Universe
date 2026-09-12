# Basketballverse — v0.97.40

## Current Build

**v0.97.40 · Newspaper Award Portraits**

## Changes in v0.97.40

- Adds the MVP’s portrait to the Championship Edition newspaper.
- Adds the Rookie of the Year’s portrait to the Championship Edition newspaper.
- Adds the first overall draft pick’s portrait to the Season Preview Edition newspaper.
- Displays the first pick’s drafting team beside the portrait.
- Uses the same `portraits/` folder, explicit portrait keys, and fallback behavior as the rest of Basketballverse.
- Backfills the first-overall portrait when an existing saved Season Preview is opened from the Newspaper Archive.
- Keeps the natural generated-player name repair from v0.97.39.
- Updates the home-page version and persistent watermark to v0.97.40.

## Portrait Placement

- **Championship Edition:** MVP and Rookie of the Year appear beneath the champion headline.
- **Season Preview Edition:** the first overall pick appears above the draft recap.
- If an image is unavailable, the newspaper displays the player’s initials instead of a broken image.

## Test Checklist

- Finish a season and confirm portraits appear for MVP and Rookie of the Year.
- Finish the draft and confirm the first overall pick’s portrait and drafting team appear in the Season Preview.
- Open both editions from History → Newspapers and confirm the portraits still appear.
- Confirm players with explicit portrait keys load the intended `.webp` files.
- Confirm a missing portrait falls back cleanly to initials.

## Repository Structure

```text
Basketball-Universe/
├── index.html
└── README.md
```

Keep the existing `logos/`, `portraits/`, and other asset folders in the GitHub repository. Replace only `index.html` and `README.md` with the files from this update.

## Save Compatibility

Existing browser saves remain compatible. Newspaper editions are enhanced when rendered; no existing portrait files or player records are changed.
