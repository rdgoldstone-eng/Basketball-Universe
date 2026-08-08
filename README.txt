v0.45 Basketball Universe — Rookie Simulation & 1988 Draft

SIMULATION INTEGRITY FIX
Drafted/generated players were created with an empty historical stat object containing zero per-36 values.
Because zero is technically a valid number, the simulation could mistake those placeholders for real historical production and give a rookie a near-zero statistical profile.

v0.45 fixes that.

A player's historical per-36 profile is now used only when he actually has a historical sample (games or minutes).
Otherwise, the game derives his scoring, rebounding, assists, steals, and blocks profile from his ratings and position.

WHY THIS MATTERS
- elite prospects can actually produce like elite prospects
- rookies are no longer suppressed by zero historical placeholders
- Rookie of the Year races become much healthier
- alternate-history development is less dependent on real-life future stats
- Jordan/Olajuwon/etc. still are not hardcoded award winners; they simply get to perform from their simulated ratings

1988 DRAFT CLASS
The historical pipeline now includes 1988, led by:
Danny Manning, Rik Smits, Charles Smith, Chris Morris, Mitch Richmond, Hersey Hawkins, Rex Chapman, Rony Seikaly, Rod Strickland, Dan Majerle, and others.

Prospect ratings reflect draft-time perception rather than eventual career hindsight.

DRAFT PIPELINE HEALTH
Scouting now shows whether the upcoming historical class is installed.
If the next class is missing, the game explicitly says so rather than silently recycling the prior year's class.

GitHub update:
Upload index.html and README.txt over the current files and commit.
