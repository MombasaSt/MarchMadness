Raw file header definitions:

**Year** - The season the team played in

**Team** - The university's D1 college basketball team participating in the tournament

**Seed** - The seed given to the team by the panel that created the season's bracket. There are 4 regions in the bracket that each have 16 seeds.
  *Note: While there have been 1-4 play-in games since 2001, these play-in games are ignore for this exercise, as the seeds that are in the play-in games has changed by year, and do not affect the round of 64/going forward.*
  
**Conf** - The conference the team played in that season

**W** - Games the team won before the tournament

**L** - Games the team lost before the tournament

**AdjEM** - Adjusted efficiency margin - a team's AdjO-AdjD

**AdjEM-Rk** - The team's rank in AdjEM on the season

**AdjO** - Adjusted offensive efficiency – An estimate of the offensive efficiency (points scored per 100 possessions) a team would have against the average D-I defense.

**AdjO-Rk** - The team's rank in AdjO on the season

**AdjD** - Adjusted defensive efficiency – An estimate of the defensive efficiency (points allowed per 100 possessions) a team would have against the average D-I offense.

**AdjD-Rk** - The team's rank in AdjD on the season

**AdjT** - Adjusted tempo – An estimate of the tempo (possessions per 40 minutes) a team would have against the team that wants to play at an average D-I tempo.

**AdjT-Rk** - The team's rank in AdjT on the season

**Luck** - From Ken's website: "A measure of the deviation between a team’s actual winning percentage and what one would expect from its game-by-game efficiencies...Essentially, a team involved in a lot of close games should not win (or lose) all of them. Those that do will be viewed as lucky (or unlucky)."

**Luck-Rk** - The team's rank in Luck on the season

**SOS-AdjEM**, **SOS-AdjEM-Rk**, **SOS-OppO**, **SOS-OppO-Rk**, **SOS-OppD**, **SOS-OppD-Rk** - The total efficiency of the opponents that the team played on the year, where better/higher is a more difficult schedule; the statistics are the reflected versions of the team's adjusted statistics (SOS = "strength of schedule")

**NCSOS-AdjEM**, **NCSOS-AdjEM-Rk** - Same as above, but only for the non-conference strength of schedule

**R64-Opp-Seed** - The seed the team played in the Round of 64. This will always be the absolute value of Seed-17

**R64-Res** - The result of the team playing in the Round of 64.
  W: Win
  L: Loss
  This is the target variable.
