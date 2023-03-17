Raw file header definitions:

**YearTeam** - The season the team played in & the university's D1 college basketball team participating in the tournament

**Seed** - The seed given to the team by the panel that created the season's bracket. There are 4 regions in the bracket that each have 16 seeds.
  *Note: While there have been 1-4 play-in games since 2001, these play-in games are ignored for this exercise, as the seeds that are in the play-in games has changed by year, and do not affect the round of 64/going forward.*
  
**Conf** - The conference the team played in that season

1: ACC
  
2: America East

3: American

4: Atlantic 10

5: Atlantic Sun

6: Big 12

7: Big East

8: Big Sky

9: Big South

10: Big Ten

11: Big West

12: CAA

13: C-USA

14: Horizon

15: Ivy League

16: MAAC

17: MAC

18: MEAC

19: Missouri Valley

20: Mountain West

21: Northeast

22: Ohio Valley

23: Pac-12 (formerly Pac-10)

24: Patriot

25: SEC

26: Southern

27: Southland

28: Summit (formerly Mid-Continent)

29: Sun Belt

30: SWAC

31: WAC

32: West Coast

**G** - Games the team played

**W-L%** - Win-loss percentage for the team; calculated as W/(W+L)

**ConfW-L%** - Record in conference play
  
**HomeW-L%** - Record when playing at home
    
**AwayW-L%** - Record when playing away from home (not at a neutral site)
 
**AdjEM** - Adjusted efficiency margin - a team's AdjO-AdjD

**AdjO** - Adjusted offensive efficiency – An estimate of the offensive efficiency (points scored per 100 possessions) a team would have against the average D-I defense.

**AdjD** - Adjusted defensive efficiency – An estimate of the defensive efficiency (points allowed per 100 possessions) a team would have against the average D-I offense.

**AdjT** - Adjusted tempo – An estimate of the tempo (possessions per 40 minutes) a team would have against the team that wants to play at an average D-I tempo.

**Luck** - From Ken's website: "A measure of the deviation between a team’s actual winning percentage and what one would expect from its game-by-game efficiencies...Essentially, a team involved in a lot of close games should not win (or lose) all of them. Those that do will be viewed as lucky (or unlucky)."

**SOSAdjEM**, **SOSOppO**, **SOSOppD** - The total efficiency of the opponents that the team played on the year, where better/higher is a more difficult schedule; the statistics are the reflected versions of the team's adjusted statistics (SOS = "strength of schedule")

**NCSOSAdjEM** - Same as above, but only for the non-conference strength of schedule

**R64Res** - The result of the team playing in the Round of 64.

  1: Win
  
  0: Loss
  
  This is the target variable.
