# Basketballverse v0.96.40
## Draft Room Player Portraits

Built directly from v0.96.39.

The Draft Room now loads the actual player image files you already placed in
the /portraits folder.

Filename convention:
first_last.webp

Examples:
- clifton_mcneely.webp
- red_rocha.webp
- wataru_misaka.webp
- larry_bird.webp

The Draft Room does not generate or embed new images. It requests the existing
file at:
portraits/<normalized_player_name>.webp

If a file is missing, initials remain visible as the fallback.

The permanent Sim This Pick / Sim Rest of Draft controls from v0.96.39 are retained.
