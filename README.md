# Basketballverse — v0.97.38

## Current Build

**v0.97.38 · Two-Edition Newspaper Cycle**

## Changes in v0.97.38

- Splits the Basketballverse Chronicle into two permanent editions for every completed season.
- Shows the **Championship Edition** immediately after the champion is crowned and before entering the offseason.
- Championship coverage includes the regular-season leaders, award winners, postseason result, champion, runner-up, and Finals MVP.
- Shows the **Season Preview Edition** after the offseason is complete and before the next season begins.
- Preview coverage includes major draft picks and rookies, trades, signings, retirements, relocations, expansion, rebranding, and realignment news.
- Each edition appears only once during progression and is saved separately in the Newspaper Archive.
- Preserves the existing offseason checklist and next-season readiness checks.
- Keeps the Minneapolis Lakers historical-logo repair from v0.97.37.
- Updates the home-page version and persistent build watermark to v0.97.38.

## Newspaper Timing

1. Finish the playoffs and crown a champion.
2. Open the Offseason to read the Championship Edition.
3. Complete every offseason stage through **Next Season**.
4. Select **Start Next Season** to read the Season Preview Edition.
5. Select the newspaper's start-season button to advance to opening night.

## Test Checklist

- Finish a season and confirm the Championship Edition appears before the offseason.
- Confirm the first paper contains championship and award coverage but no offseason recap.
- Complete the offseason and select Start Next Season.
- Confirm the Season Preview Edition appears before the year changes.
- Confirm its button starts the next season exactly once.
- Open History → Newspapers and confirm both editions are selectable.
- Save and reload at each newspaper checkpoint to confirm neither edition loops.

## Repository Structure

```text
Basketball-Universe/
├── index.html
└── README.md
```

Keep the existing `logos/`, `portraits/`, and other asset folders in the GitHub repository. Replace only `index.html` and `README.md` with the files from this update.

## Save Compatibility

Existing browser saves remain compatible. New two-edition newspaper history is added to the save as seasons are completed.
