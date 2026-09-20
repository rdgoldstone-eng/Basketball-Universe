# Basketballverse — v0.97.70

## Current Build

**v0.97.70 · Franchise Market Decisions**

## Changes in v0.97.70

- Adds a Commissioner market report beside relocation and expansion choices. It shows the last available U.S. city census count at the selected year, franchise attendance, stability, and relocation pressure. It records approved franchise changes in this universe’s timeline and in the existing news feed.
- Uses the dated city population as one input to expansion bid scores and opening fan support, and adds modest relocation pressure for small cities alongside attendance, results, and stability. The Commissioner may still approve or decline the proposed changes. City boundaries are not metropolitan areas; the interface identifies this explicitly. Markets without a comparable count use existing gameplay scores without invented population figures.
- Displays the champion’s historical team logo beside each title in League → History, with a fallback if that team’s image is unavailable.
- Preserves existing saved universes and earlier offseason fixes. Updates the page banner, watermark, and build metadata.

## Population source and limitations

U.S. Census Bureau, Campbell Gibson, *Population of the 100 Largest Cities and Other Urban Places in the United States: 1790 to 1990*, Working Paper 27, [tables 18–22](https://www2.census.gov/library/working-papers/1998/demo/pop-twps0027/twps0027.html). Values are 1950, 1960, 1970, 1980 or 1990 city / urban-place census counts. In between censuses the game shows the latest actual observation, marked with its census year. Data older than 19 years do not influence the market score. U.S. markets outside the source’s top 100 and Canadian or Mexican markets have no sourced count in this release. City boundary changes (notably Nashville) can change counts independently of population growth. Metro-area demographic modelling is a future data step.

## Installation

Replace the repository-root `index.html` and `README.md` with the files in this ZIP. Keep existing `portraits/`, `logos/`, and other asset folders. Browser saves stay in place.
