# Basketballverse v0.96.07
## Historical Branding Timeline — 1960–1976
**CURRENT BUILD: v0.96.07**

Built directly from v0.96.06. The 1946–1959 historical branding timeline remains installed.

This section extends the year-aware historical identity/logo resolver through 1976.
It includes the major relocation/name transitions:
Minneapolis -> Los Angeles Lakers;
Philadelphia -> San Francisco -> Golden State Warriors;
Syracuse Nationals -> Philadelphia 76ers;
St. Louis -> Atlanta Hawks;
Chicago Packers -> Chicago Zephyrs -> Baltimore/Capital/Washington Bullets;
San Diego -> Houston Rockets;
Cincinnati -> Kansas City-Omaha -> Kansas City Kings.

It also adds expansion-era identity slots for Chicago Bulls, Seattle SuperSonics,
Milwaukee Bucks, Phoenix Suns, Cleveland Cavaliers, Buffalo Braves, Portland Trail
Blazers and New Orleans Jazz.

Historical artwork filenames are listed in:
logos/historical/LOGO_TIMELINE_1960_1976.csv

The artwork is intentionally externalized into logos/historical/*.webp. The game
selects the correct file automatically by identity and simulated year. Missing artwork
falls through the existing UI fallback rather than breaking the page.

Alternate-history rule remains unchanged: once a franchise diverges from its real
identity through an in-universe move/rebrand, real-world future branding is not forced.
