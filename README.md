# Basketballverse v0.97.02
## Recovery Baseline — Visible Build Identity Fix

Important finding:
v0.97.01 *was intentionally using the exact v0.96.39 runtime* so we could return
to the last confirmed-working game. The startup page and footer, however, had
already rendered the old v0.96.39 label before the final recovery metadata ran.
That made a newly uploaded recovery build look exactly like the old build.

v0.97.02 keeps the same confirmed-working runtime and explicitly refreshes the
visible build label after the page has loaded.

If GitHub Pages is serving this file, the page will visibly show:
v0.97.02 · Recovery Baseline

No gameplay behavior is changed in this version.
