# Basketballverse — v0.97.71

## Current Build

**v0.97.71 · Custom Franchise Logos**

## Changes in v0.97.71

- Commissioner → League Office → Expansion & Relocation now offers a custom city, nickname and PNG/JPG/WebP logo upload in the same screen as franchise approvals. Choose “Use for Relocation” or “Use for Expansion” to create and select an identity, then review and approve the actual transaction above it.
- Adds a logo preview for the selected relocation or expansion identity. Built-in teams use their identity’s era logo or historical logo. A newly created identity uses its uploaded image in every era.
- Compresses uploads to a transparent-capable WebP image up to 512 pixels before storing them in the universe save. Images too large for a browser save prompt for a smaller file. The franchise and its identity history retain the custom logo after approval.
- Blocks a relocation identity already being used by a different active team. Expansion still blocks names already in use.
- Includes the v0.97.70 population-based market report and champion logos in League History. Updates the visible build banner, watermark and version metadata.

## Example: Move the Pistons to South Bend

1. As Commissioner, open League Office → Expansion & Relocation.
2. Select the existing Pistons in “Relocate Existing Franchise.”
3. Under “Build a Custom Franchise Identity,” enter **South Bend**, **Pistons**, and select your image. Wait for the logo preview.
4. Select **Use for Relocation**. The South Bend market and identity are selected above, with its logo preview.
5. Select **Approve Relocation** and confirm.

The uploaded image is saved inside that game universe in your browser and in exported save games. It is not uploaded to your GitHub `logos/` folder; other people need that saved universe or a separately hosted logo asset to see it. Keep a backup of your save before clearing browser data.

## Installation

Replace the repository-root `index.html` and `README.md` with the files in this ZIP. Keep existing `portraits/`, `logos/`, and other asset folders.
