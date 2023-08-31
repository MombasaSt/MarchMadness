## Dataset Description

The raw file *History-MM-Raw.xlsx* in this depository lists numerous team, singular-opponent, season-opponent, and differential statistics for every team that has played in the Round of 64 of the NCAA Men's Division I College Basketball Tournament, colloquially known as "March Madness", from 2010 to 2022. Years prior are left out due to tournament changes and missing advanced data, and 2023 is not included due to the recency of the data compared to the project's beginning.

All traditional and advanced statistics (from the leftmost column to *SOS_Diff*) in the file are from Basketball Reference, run by Sports Reference LLC; all adjusted statistics (from *AdjEM* to *NCSOSAdjEM_Diff*) are from KenPom, run by Ken Pomeroy. The last column is the readily-available statistic of whether the team won their first round matchup or not.

## Statistics: Suffixes

Preceding this section are the definitions for each of the "base" columns/statistics present in the raw dataset. There are 4 suffixes, preceded by an underscore (_), that are also present; the reasoning for these suffixes are as follows, with examples below each using the first row:

**No underscore/suffix** - This is the "base" statistic/value of the team being represented majorly on the record in the table. Additionally, these are all the statistics defined below.  
*Ex: In the first row of data, for column **PPG**, or **Points Per Game**, this is the amount of points per game Cal Poly scored on average, which was 62.97.*

**Suffix of _R64Opp** - This is the corresponding base statistic for the opponent of the team assigned to the current row.  
*Ex: In the first row of data, for column **PPG_R64Opp**, or **Points Per Game by Round of 64 Opponent**, this is the amount of points per game Wichita State scored on average, which was 75.17.*

**Suffix of _SznOpp** - This is the corresponding base statistic for all the opponents the team assigned to the current row faced.  
*Ex: In the first row of data, for column **PPG_SznOpp**, or **Points Per Game by Season Opponents**, this is the amount of points per game Cal Poly allowed to their opponents, which was 63.62.*

**Suffix of _Diff_R64Opp** - This is the difference between the base statistic and the Round of 64 opponent's base statistic.  
*Ex: In the first row of data, for column **PPG_Diff_R64Opp**, or **Difference in Points Per Game from Round of 64 Opponent**, this is the difference between Cal Poly and Wichita State's PPG, which is -12.2 (62.97-75.17).*

**Suffix of _Diff_SznOpp** - This is the difference between the base statistic and the season opponents' base statistic.  
*Ex: In the first row of data, for column **PPG_Diff_SznOpp**, or **Difference in Points Per Game from Season Opponents**, this is the difference between Cal Poly and their season opponents' PPG, which is -0.65 (62.97-63.62).*

## Statistics: Base Statistics

Presented below are all the base statistics in the table. Suffixed statistics are not included.

**Year** - The season the team played in.  
  *Note: If the season being played was 2013-2014, the year present is 2014. This follows traditional statistical conventions used in sports analytics for sports that include a season that runs between years.*

**College** - The college's basketball team being analyzed
  
**Conf** - The conference the team played in that season
  
**Seed** - The seed given to the team by the panel that created the season's bracket. There are 4 regions in the bracket that each have 16 seeds.  
  *Note: While there have been 1-4 play-in games since 2001, these play-in games are ignored for this exercise, as the seeds that are in the play-in games has changed by year, and do not affect the round of 64/going forward.*

**Stats go here**

**R64Res** - The result of the team playing in the Round of 64. A 1 represents a win and a 0 a loss. This is the target variable.
