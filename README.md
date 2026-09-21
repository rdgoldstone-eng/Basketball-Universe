# Basketballverse — v0.97.72

## Current Build

**v0.97.72 · Relocation City Builder**

## Changes in v0.97.72

- Commissioner → League Office → Expansion & Relocation now handles a move in one form: select the existing team, search and choose a destination from a list of more than 130 cities, edit its team nickname, upload a PNG/JPG/WebP logo, preview the new identity, then approve the relocation. South Bend is included.
- Selecting the team fills the nickname field with its current nickname: Detroit Pistons defaults to **Pistons**. Selecting South Bend makes the preview **South Bend Pistons**. You may type a different nickname before approval.
- The logo upload is required before relocation approval. Images are resized to a maximum of 512 pixels and encoded as WebP where supported. The confirmation names the origin team and proposed destination. Existing teams cannot share the same full name.
- Moving a team retains its franchise ID and roster, updates players to the new team name, and records its old and new identities and market in the saved universe. The custom image is stored once in the save and restored into team and franchise history when loaded, reducing browser storage use.
- The separate custom identity form remains available for expansion. Expanding still creates a new franchise and runs the expansion draft.
- Adds the documented 1950 and 1960 South Bend U.S. Census city counts to the market report. The list contains more destinations than the population dataset; unsourced cities have no fabricated population estimate.
- Keeps v0.97.70 champion logos and market data and v0.97.71 upload support. Updates banner, watermark and metadata to v0.97.72.

## Example: Detroit to South Bend

1. Open **Commissioner → League Office → Expansion & Relocation**.
2. Select **Detroit Pistons**. The team name field fills with **Pistons**.
3. Search for and select **South Bend**.
4. Upload the new logo. Wait for its preview, then choose **Approve Relocation** and confirm.

The upload is included in that universe's browser save and exported save game; it does not automatically add a file to the GitHub repository's `logos/` folder. Keep an exported save before clearing browser data.

## Population source

U.S. Census Bureau, Campbell Gibson, *Population of the 100 Largest Cities and Other Urban Places in the United States: 1790 to 1990*, Working Paper 27, [tables 18–22](https://www2.census.gov/library/working-papers/1998/demo/pop-twps0027/twps0027.html). South Bend's city population was 115,911 in 1950 and 132,445 in 1960. These are city counts, not metro area counts.

## Installation

Replace the repository-root `index.html` and `README.md` with the files in this ZIP. Keep the existing `portraits/`, `logos/`, and other asset folders. Existing saves remain in place.
