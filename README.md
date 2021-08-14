# MLB historical WAR data

The file *"jeffbagwell_war_historical.csv"* contains wins above replacement (WAR) data -- according to [JEFFBAGWELL](https://fivethirtyeight.com/features/can-we-play-nba-jam-with-mlb-teams/) (the **J**oint **E**stimate **F**eaturing **F**anGraphs and **B**-R **A**ggregated to **G**enerate **W**AR, **E**qually **L**eveling **L**ists), which averages together WAR from Baseball-Reference.com and FanGraphs -- plus various other metrics for MLB since 1901.

Note that this file includes players from the Negro Leagues recently added to Baseball-Reference's database. For those players (and any others without matching FanGraphs IDs/stat entries), Baseball-Reference data is used solely for WAR and the various run values, and "+" stats (indexed to league average) are not currently available.


|   Category    |                                              Description                                              |
|---------------|-------------------------------------------------------------------------------------------------------|
| player_name   | Player's name.                                                                                        |
| age           | Player's age as of July 1.                                                                            |
| key_bbref     | Player's Baseball-Reference ID.                                                                       |
| year_ID       | Season.                                                                                               |
| team_ID       | Team played for.                                                                                      |
| stint_ID      | Stint no. (i.e., order of teams played for).                                                          |
| lg_ID         | League played in.                                                                                     |
| is_P          | Was the player a pitcher? Y/N (May be incomplete.)                                                        |
| franch_ID     | Franchise played for (uses Lahman DB ID).                                                             |
| sched         | No. of scheduled games for team.                                                                      |
| g_bat         | Games as a batter.                                                                                    |
| pa            | Plate appearances.                                                                                    |
| bat162        | Batting runs above avg. per 162 team games.                                                           |
| bsr162        | Baserunning runs above avg. per 162 team games.                                                       |
| fld162        | Fielding runs above avg. per 162 team games.                                                          |
| pos162        | Positional runs above avg. per 162 team games.                                                        |
| def162        | Defense runs above avg. (includes fielding and positional adjustment) per 162 team games.             |
| rep162        | Replacement runs per 162 team games.                                                                  |
| bwar162       | JEFFBAGWELL batter WAR per 162 team games.                                                            |
| BB_plus       | Batting walk rate indexed relative to league average (which is always 100).                           |
| K_plus        | Batting strikeout rate indexed relative to league average (which is always 100).                      |
| AVG_plus      | Batter's batting average indexed relative to league average (which is always 100).                    |
| OBP_plus      | On-base percentage indexed relative to league average (which is always 100).                          |
| SLG_plus      | Slugging percentage indexed relative to league average (which is always 100).                         |
| wRC_plus      | Weighted runs per PA indexed relative to league average (which is always 100).                        |
| ISO_plus      | Isolated power indexed relative to league average (which is always 100).                              |
| BABIP_plus    | Batter's batting average on balls in play indexed relative to league average (which is always 100).   |
| LD_plus       | Batter's line drive rate indexed relative to league average (which is always 100).                    |
| GB_plus       | Batter's groundball rate indexed relative to league average (which is always 100).                    |
| FB_plus       | Batter's flyball rate indexed relative to league average (which is always 100).                       |
| Pull_plus     | Rate of batted balls to pull side, indexed relative to league average (which is always 100).          |
| Cent_plus     | Rate of batted balls up the middle, indexed relative to league average (which is always 100).         |
| Oppo_plus     | Rate of batted balls to the opposite field, indexed relative to league average (which is always 100). |
| g_pitch       | Games as a pitcher.                                                                                   |
| starts        | Games as a starting pitcher.                                                                          |
| innings       | Innings pitched.                                                                                      |
| relief_pct    | Share of innings in relief.                                                                           |
| avg_LI        | Average leverage index of appearances.                                                                |
| br_pwar162    | Baseball-Reference pitching WAR per 162 games.                                                        |
| fg_pwar162    | FanGraphs pitching WAR per 162 games.                                                                 |
| ra9_pwar162   | Runs-allowed-per-9 based pitching WAR per 162 games.                                                  |
| pwar162       | JEFFBAGWELL pitcher WAR per 162 games.                                                                |
| K9_plus       | Pitching strikeouts per 9 innings, indexed relative to league average (which is always 100).          |
| BB9_plus      | Pitching walks per 9 innings, indexed relative to league average (which is always 100).               |
| KBB_plus      | Strikeout to walk ratio indexed relative to league average (which is always 100).                     |
| HR9_plus      | Home runs allowed per 9 innings, indexed relative to league average (which is always 100).            |
| Kpct_plus     | Pitching strikeout rate indexed relative to league average (which is always 100).                     |
| BBpct_plus    | Pitching walk rate indexed relative to league average (which is always 100).                          |
| oppAVG_plus   | Opponent's batting average indexed relative to league average (which is always 100).                  |
| WHIP_plus     | Walks plus hits divided by innings pitched, indexed relative to league average (which is always 100). |
| oppBABIP_plus | Opponent's batting average on balls in play indexed relative to league average (which is always 100). |
| LOB_plus      | Left on base percentage allowed, indexed relative to league average (which is always 100).            |
| ERA_minus     | Earned run average indexed relative to league average (which is always 100).                          |
| FIP_minus     | Fielding independent pitching indexed relative to league average (which is always 100).               |
| xFIP_minus    | Expected fielding independent pitching indexed relative to league average (which is always 100).      |
| oppLD_plus    | Opponent's line drive rate indexed relative to league average (which is always 100).                  |
| oppGB_plus    | Opponent's groundball rate indexed relative to league average (which is always 100).                  |
| oppFB_plus    | Opponent's flyball rate indexed relative to league average (which is always 100).                     |
| pct_PT        | Share of team playing time (based on PA and batters faced, adjusted for leverage).                    |
| WAR162        | JEFFBAGWELL WAR per 162 team games.                                                                   |
| gms_P         | Appearances as a pitcher.                                                                             |
| gms_C         | Appearances as a catcher.                                                                             |
| gms_1B        | Appearances as a first baseman.                                                                       |
| gms_2B        | Appearances as a second baseman.                                                                      |
| gms_3B        | Appearances as a third baseman.                                                                       |
| gms_SS        | Appearances as a shortstop.                                                                           |
| gms_LF        | Appearances as a left fielder.                                                                        |
| gms_CF        | Appearances as a center fielder.                                                                      |
| gms_RF        | Appearances as a right fielder.                                                                       |
| gms_OF        | Appearances as an outfielder.                                                                         |
| gms_DH        | Appearances as a designated hitter.                                                                   |
| gms_PH        | Appearances as a pinch hitter.                                                                        |
| gms_PR        | Appearances as a pinch runner.                                                                        |
| prev_tm       | Previous franchise played for.                                                                        |
| arrived       | First season with franchise.                                                                          |
| departed      | Last season with franchise.                                                                           |
| next_tm       | Next franchise played for.                                                                            |
| salary        | Salary earned that season (very incomplete before the 1990s).                                         |
