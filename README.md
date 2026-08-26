# Basketballverse v0.96.41
## Core Draft Portrait Loader

This update changes the ORIGINAL Draft Room prospect row itself instead of
trying to redraw the Draft Room afterward.

Portrait convention is now enforced globally as:
portraits/first_last.webp

Examples:
- portraits/clifton_mcneely.webp
- portraits/andy_phillip.webp
- portraits/carl_braun.webp
- portraits/red_rocha.webp
- portraits/wataru_misaka.webp

The portrait cell is part of each draft prospect row, so legacy Draft Room
renderers cannot erase it without rendering the same portrait-enabled row again.

Older portrait code that tried first-last.webp is overridden at the end of the
build so the game consistently uses the underscore filenames already uploaded
to the /portraits folder.

The permanent Draft simulation controls from v0.96.39 remain intact.
