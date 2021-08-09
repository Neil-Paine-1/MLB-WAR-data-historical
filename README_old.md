**Note (Aug. 9, 2021):** *This is an old version of the readme for the historical dataset. The file mlb-war-data-historical.csv is out of date.*


# MLB historical WAR data

**Note (Jul. 14, 2021):** *The combined Baseball-Reference/FanGraphs data here is out of date. After Baseball-Reference [added players from the Negro Leagues to its official MLB data](https://www.baseball-reference.com/negro-leagues-are-major-leagues.shtml) on June 15, I decided to pause JEFFBAGWELL updates until FanGraphs also adds those players. This is simply to keep the historical record from being extremely incomplete, with a vast number of players not able to have matching B-R and FG IDs and not existing in half of the datasets used.*

The file "mlb-war-data-historical.csv" contains wins above replacement (WAR) data -- according to [JEFFBAGWELL](https://fivethirtyeight.com/features/can-we-play-nba-jam-with-mlb-teams/) (the Joint Estimate Featuring FanGraphs and B-R Aggregated to Generate WAR, Equally Leveling Lists), which averages together WAR from Baseball-Reference.com and FanGraphs -- plus various other metrics for MLB since 1901.



|  Category   |                            Description                            |
|-------------|-------------------------------------------------------------------|
| name_common | Player name                                                       |
| age         | Age as of Jul. 1                                                  |
| player_ID   | Baseball-Reference ID                                             |
| year_ID     | Season                                                            |
| team_ID     | Team abbreviation                                                 |
| lg_ID       | League                                                            |
| PA          | Plate appearances                                                 |
| IP          | Innings pitched                                                   |
| bWAR        | Batter wins above replacement (incl. defense)                     |
| pWAR        | Pitcher wins above replacement                                    |
| WAR         | Wins above replacement                                            |
| BB_pct      | Walk rate (batting)                                               |
| K_pct       | Strikeout rate (batting)                                          |
| ISO         | Isolated power                                                    |
| BABIP.x     | Batting AVG on balls in play (batting)                            |
| Spd         | Speed Score                                                       |
| wRCp        | Weighted Runs Created+                                            |
| BRRAA       | Baserunning runs above avg                                        |
| DRAA        | Defensive runs above avg (incl. position adjustment)              |
| K9          | Strikeouts/9 innings (pitching)                                   |
| BB9         | Walks/9 innings (pitching)                                        |
| HR9         | Home runs/9 innings (pitching)                                    |
| BABIP.y     | Batting AVG on balls in play (pitching)                           |
| LOB_pct     | % of runners left on base (pitching)                              |
| ERAm        | Earned Run Average-                                               |
| FIPm        | Fielding Independent pitching-                                    |
| gmLI        | Avg Leverage index entering game                                  |
| pct_PT      | Share of total team playing time                                  |
| WAR162      | WAR per 162 team games                                            |
| def_pos     | Primary defensive position (will not include DH)                  |
| FWS         | "Faux Win Shares" - WAR re-scaled to mimic Bill James' Win Shares |
| fr_lahman   | Franchise ID (according to Sean Lahman's database)                |
| Prev Tm     | Previous franchise played for                                     |
| Arrived     | First year w/ current franchise                                   |
| Departed    | Final year w/ current franchise                                   |
| Next Tm     | Following franchise played for                                    |



