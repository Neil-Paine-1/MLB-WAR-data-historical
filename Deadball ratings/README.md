# Deadball player ratings

This CSV contains historical MLB player ratings for the wonderful tabletop game [Deadball: Baseball With Dice](https://www.kickstarter.com/projects/wmakers/deadball-baseball-with-dicesecond-edition) by W.M. Akers. The game comes with many fictional players, teams and leagues, but there is also a guide to creating ratings for real-life players using sabermetric statistics, which I have applied here with the help of [FanGraphs' "Plus" stats](https://www.fangraphs.com/leaders.aspx?pos=all&stats=bat&lg=all&qual=y&type=23&season=2022&month=0&season1=2022&ind=0&team=0&rost=0&age=0&filter=&players=0&startdate=2022-01-01&enddate=2022-12-31), which normalize a player's statistics relative to the league average. (Player stats were normalized to a generic MLB season with averages that match the long-term historical norms, with a slight emphasis on the playing environment since 2000.) These ratings are for AL and NL players -- players from the Negro Leagues or Federal League were not included because of data limitations -- since 1901, for those who met the minimum criteria of either 100 plate appearances or 20 innings pitched per 162 team games for the whole season in question. (Players who were on multiple teams will be listed with all of their teams.) Pitchers who did not log 100 PAs were assigned a BT of 15 and an OBT of 19 when batting, with negative batting traits -- although it is recommended to ignore their C- contact trait for the purposes of bunting (since pitchers used to practice bunting a lot).


|   Category    |                                             Description                                             |
|---------------|-----------------------------------------------------------------------------------------------------|
| key_bbref     | Player's ID at Baseball-Reference                                                                   |
| player_name   | Player's name                                                                                       |
| year_ID       | Season                                                                                              |
| team_ID       | Team                                                                                                |
| pos1          | Primary position (by most games)                                                                    |
| pos2          | Secondary position (for players who had at least 20% of their games at a non-primary pos)           |
| hand          | Handedness -- batting or pitching, or B/T when a pitcher bats with a different hand than they throw |
| age           | Age as of June 30                                                                                   |
| bt            | Batting Target (based on normalized batting average)                                                |
| obt           | On-Base Target (based on normalized OBP)                                                            |
| power         | Power trait (based on ISO+)                                                                         |
| contact       | Contact trait (based on K%+)                                                                        |
| speed         | Speed trait (based on JEFFBAGWELL baserunning runs/162)                                             |
| defense       | Defense trait (based on JEFFBAGWELL defensive runs/162)                                             |
| tough         | Toughness trait (based on career games played per 162)                                              |
| pitch_die     | Pitcher's Pitch Die level (based on normalized ERA)                                                 |
| strikeout     | Strikeout trait (based on K/9+)                                                                     |
| control       | Control trait (based on BB/9+)                                                                      |
| groundball    | Groundball trait (based on GB%+ or a combo of ERA- and K/9+ for older eras)                         |
| stamina       | Stamina trait (based on innings pitched per 162)                                                    |
| is_P          | Pitcher tag                                                                                         |
| is_SP         | Starting pitcher tag                                                                                |
| season_PA     | Player's plate appearances per 162 team games across all teams played for                           |
| season_IP     | Player's innings pitched per 162 team games across all teams played for                             |
| season_pct_PT | Player's total share of team playing time across all teams played for                               |

