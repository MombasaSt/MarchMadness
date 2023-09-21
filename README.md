## Dataset Description

The raw file *HistoryMMRaw.csv* in this depository lists numerous team, singular-opponent, season-opponent, and differential statistics for every team that has played in the Round of 64 of the NCAA Men's Division I College Basketball Tournament, colloquially known as "March Madness", from 2010 to 2022. Years prior are left out due to the tournament having a different format beforehand and missing advanced data for that time period, while 2023 is not included due to the recency of the data compared to the project's beginning.

All traditional and advanced statistics (from the leftmost column to "Pace") in the file are from Sports Reference - College Basketball, run by Sports Reference LLC; all adjusted statistics (from "AdjEM" to "NCSOSAdjEM_Diff") are from KenPom, run by Ken Pomeroy. The last column is the readily-available statistic of whether the team won their first round matchup or not.

Sports Reference - College Basketball: https://www.sports-reference.com/cbb/postseason/  
KenPom: https://kenpom.com/

## Statistics: Suffixes

Preceding this section are the definitions for each of the "base" columns/statistics present in the raw dataset. There are 4 suffixes, preceded by an underscore (_), that are also present; the reasoning for these suffixes are as follows, with examples below each using the first row:

**No underscore/suffix** - This is the "base" statistic/value of the team being represented majorly on the record in the table. Additionally, these are all the statistics defined below.  
*Ex: In the first row of data, for column **PPG**, or **Points Per Game**, this is the amount of points per game Cal Poly scored on average, which was 62.97.*

**Suffix of _R64Opp** - This is the corresponding base statistic for the opponent of the team assigned to the current row.  
*Ex: In the first row of data, for column **PPG_R64Opp**, or **Points Per Game by Round of 64 Opponent**, this is the amount of points per game Wichita State scored on average, which was 75.17.*

**Suffix of _SznOpp** - This is the corresponding base statistic for all the opponents the team assigned to the current row faced.  
*Ex: In the first row of data, for column **PPG_SznOpp**, or **Points Per Game by Season Opponents**, this is the amount of points per game Cal Poly allowed to their opponents, which was 63.62.*  
*Note: WLP and KenPom statistics do not have SznOpp equivalents.*

**Suffix of _Diff_R64Opp** - This is the difference between the base statistic and the Round of 64 opponent's base statistic.  
*Ex: In the first row of data, for column **PPG_Diff_R64Opp**, or **Difference in Points Per Game from Round of 64 Opponent**, this is the difference between Cal Poly and Wichita State's PPG, which is -12.2 (62.97-75.17).*

**Suffix of _Diff_SznOpp** - This is the difference between the base statistic and the season opponents' base statistic.  
*Ex: In the first row of data, for column **PPG_Diff_SznOpp**, or **Difference in Points Per Game from Season Opponents**, this is the difference between Cal Poly and their season opponents' PPG, which is -0.65 (62.97-63.62).*  
*Note: WLP and KenPom statistics do not have SznOpp equivalents, so they do not have SznOpp differences.*

## Statistics: Base Statistics

Presented below are all the base statistics in the table. Suffixed statistics are not included. Any definition of a building block of a statistic (i.e. the definition of a rebound) is inside the first appearance of it.

(A better in-depth explanation of the adjusted stats can be found here: https://www.onthebanks.com/2019/12/9/21002735/kenpom-rankings-explained-how-to-better-evaluate-rutgers-basketball-big-ten-ncaa-steve-pikiell)

**Team** - The college's basketball team being analyzed (based on the year in which they played). The year would traditionally be parsed out in a set such as this, but including it with the team name removes the requirement of combining columns for independent "ID's", so to speak.
  *Note: If the season being played was 2013-2014, the year present is 2014. This follows traditional statistical conventions used in sports analytics for sports that include a season that runs between years.*
  
**Seed** - The seed given to the team by the panel that created the season's bracket. There are 4 regions in the bracket that each have 16 seeds.  
  *Note: While there have been 1-4 play-in games since 2001, these play-in games are ignored for this exercise, as the seeds that are in the play-in games has changed by year, and do not affect the round of 64/going forward.*

**Conf** - The conference the team played in that season

**WLP** - Win-loss percentage; calculated by the amount of wins the team had divided by the number of games played

**ConfWLP** - Conference win-loss percentage; the team's win-loss percentage when playing against teams within their same conference

**HomeWLP** - Home win-loss percentage; the team's win-loss percentage when playing in their home arena

**AwayWLP** - Away win-loss percentage; the team's win-loss percentage when playing in another team's home arena

**PPG** - Points per game; the amount of points the team scored per game

**FGM** - Field goals made; the amount of field goals (shots) the team successfully shot per game

**FGA** - Field goals attempted; the amount of field goals the team shot, successful or not, per game

**FGp** - Field goal percentage; calculated by FGM/FGA

**ThreePM** - Three-pointers made; the amount of three-point field goals the team successfully shot per game

**ThreePA** - Three-pointers attempted; the amount of three-point field goals the team shot, successful or not, per game

**ThreePp** - Three-point percentage; calculated by ThreePM/ThreePA

**ThreePAr** - Three-point attempt rate; the percentage of field goal attempts that were three-point field goal attempts

**eFGp** - Effective field goal percentage; a statistic that accounts for three-point field goals being worth more than two-point field goals. Calculated by:  
![image](https://github.com/WalkingWiki41/MarchMadness/assets/51684045/c4d5a258-8015-4892-a903-797f8fcb2a3e)

**FTM** - Free throws made; the amount of free throws the team successfully shot per game

**FTA** - Free throws attempted; the amount of free throws the team shot, successful or not, per game

**FTp** - Free throw percentage; calculated by FTM/FTA

**FTr** - Free throw attempt rate; the percentage of free throw attempts per field goal attempts

**TSp** - True shooting percentage; an overarching statistic that estimates the ability to shoot the ball and successfully shoot free throws. Calculated by:  
![image](https://github.com/WalkingWiki41/MarchMadness/assets/51684045/f1138fa5-20dd-4972-b5de-704b0f39cc9c)

**TRPG** - Total rebounds per game; the number of rebounds - counted for a player when they get the ball after a missed shot - the team grabbed while on offense or defense per game

**TRBp** - Offensive rebound percentage; an estimate of the percentage of available total rebounds the team grabbed per game

**ORPG** - Offensive rebounds per game; the number of rebounds the team grabbed while on offense per game

**ORBp** - Offensive rebound percentage; an estimate of the percentage of available offensive rebounds the team grabbed per game

**APG** - Assists per game; the number of assists - counted for a player when they pass the ball to a teammate in a way that directly leads to a basket - by the team per game 

**ASTp** - Assist percentage; the percentage of field goals that were assisted on by the team

**SPG** - Steals per game; the number of steals - counted for a player when they cause an opponent to give the ball up - by the team per game

**STLp** - Steal percentage; the percentage of opponent possessions that ended with a steal by the team

**BPG** - Blocks per game; the number of blocks - counted for a player when they deflect the ball on a shot - by the team per game

**BLKp** - Block percentage; the percentage of opponent field goal attempts that were blocked by the team

**TPG** - Turnovers per game; the number of times the team turned the ball over - or gave it up - per game

**TOVp** - Turnover percentage;  out of 100, the number of plays that ended in a turnover for the team

**FPG** - Fouls per game; the number of times the team committed a foul - any infraction causing stoppage of play - per game

**Pace** - The pace of play; the number of possessions the team had per 40 minutes of game time

**AdjEM** - Adjusted Efficiency Margin; the overall ranking for Ken Pomeroy's adjusted statistics, with higher being better. Calculated by AdjO-AdjD, it determines how many points the team would outscore the average Division I team by

**AdjO** - Adjusted Offensive Efficiency; the amount of points a team would score per 100 possessions against an average Division I opponent

**AdjD** - Adjusted Defensive Efficiency; the amount of points a team would allow per 100 possessions against an average Division I opponent

**AdjT** - Adjusted Tempo; possessions per 40 minutes, adjusted per opponent

**Luck** - Luck rating; the measure of deviation between a team's actual winning percentage and what would be expected from game-by-game efficiencies. A team in many close games won't win all of them, and vice versa

**SOSAdjEM** - Adjusted Efficiency Margin for strength of schedule; the same as AdjEM, but for the opponents the team faced, which is effectively a strength of schedule rating

**SOSOppO** - Adjusted Offensive Efficiency for strength of schedule; the same as AdjO, but for the opponents the team faced, which is effectively an offensive strength of schedule rating

**SOSOppD** - Adjusted Defensive Efficiency for strength of schedule; the same as AdjD, but for the opponents the team faced, which is effectively a defensive strength of schedule rating

**NCSOSAdjEM** - Adjusted Efficiency Margin for non-conference strength of schedule; the same as SOSAdjEM but for teams not in the same conference

**R64Res** - The result of the team playing in the Round of 64. A 1 represents a win and a 0 a loss. This is the target variable
