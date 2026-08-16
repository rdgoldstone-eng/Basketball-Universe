# Basketballverse v0.91.50 — GM Career History Recovery

## What this fixes
Older Basketballverse saves can have years of league history — including championships — from before the GM Career Profile existed. Previous builds only backfilled seasons that already had a GM review/history entry, so those older accomplishments could display as zero.

v0.91.50 reconstructs the GM résumé from the permanent universe data already in the save.

## GM Career Profile now recovers
- Championships
- NBA Finals appearances
- Playoff appearances
- Seasons as GM
- Regular-season wins and losses when archived franchise records are available
- Career win percentage
- Best regular-season record
- Season-by-season résumé

## Legacy-save behavior
If an older save has no historical GM job-change records, Basketballverse uses the human GM's currently controlled franchise as the historical franchise for the missing years. This is the best available reconstruction for saves created before GM job history was stored.

If a save *does* contain GM job/team-change history, those explicit records take priority.

## Other fixes retained
- v0.91.49 GM playoff-objective hierarchy fix
- v0.91.48 historical first-round playoff format fix
- Free-agency economy improvements
- Draft lottery stability
- Historic newspaper context

## Version
In-game build banner: **v0.91.50 · GM Career History Recovery**

## Test
Load your existing long-running GM save and open the Career section. Your previously won championships should now appear in the GM Career totals and in the season-by-season résumé without starting a new universe.
