v0.43.1 Basketball Universe — Embedded Merger Era Logos

FIX
v0.43 used external historical-logo URLs. Those requests could fail in the browser, causing Basketball Universe to fall back to the generated placeholder logos.

v0.43.1 embeds all 22 real 1976-77 team logo images directly inside index.html.

RESULT
- No external hotlink is required.
- GitHub Pages serves the logo data as part of the game itself.
- Old generated logos saved by previous versions are cleared when a real embedded historical logo exists.
- The Logo Browser labels these as "Real historical · embedded".
- Generated logos remain only as emergency fallbacks.

1976-77 EMBEDDED TEAMS
Atlanta, Boston, Buffalo, Chicago, Cleveland, Denver, Detroit, Golden State, Houston, Indiana, Kansas City, Los Angeles Lakers, Milwaukee, New Orleans, New York Knicks, New York Nets, Philadelphia, Phoenix, Portland, San Antonio, Seattle, and Washington.

GitHub update:
Upload index.html and README.txt over the current files and commit.

If the browser still displays old artwork immediately after GitHub Pages deploys, reload the page once so it receives the new index.html.
