v0.68 Basketball Universe — Three Logo Framework

This build upgrades the identity system so every franchise identity can support a three-logo library:
- Early NBA
- Growing NBA
- Modern

What changed
- Every built-in identity now initializes with a three-logo library.
- Every custom identity now gets a three-logo library automatically.
- Teams now carry logo-library data, so relocations and expansions bring their era logo set with them.
- The active logo now follows year buckets:
  * Early NBA: 1946-1966
  * Growing NBA: 1967-2003
  * Modern: 2004-present
- Real / historical artwork still overrides the active in-season logo when an exact historical asset exists.
- Identities screen now previews all three logo slots for each identity.
- Logo Browser now shows both the active selected-year logo and the full three-logo library.

Notes
- This is the framework pass. For many fake/original identities, Early and Growing variants are generated in-house so every franchise has complete coverage immediately.
- Modern slots preserve existing real/current artwork when available.
- This gives every team, including fake teams, at least three library logos.
