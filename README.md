Data regarding pulling the goalie in the PWHL

I realized that at least 14 `goalie_change` events are missing from the official data, and the TOI for those goalies was not updated accordingly. 
I attempted to manually add these events. Code is in [Pulling_the_goalie.ipynb](Pulling_the_goalie.ipynb)

|   game_id | game_date                    | goalie_out_info.last_name   | time   | home_team_name   | away_team_name       | pulling_team_name    | url                                               |
|----------:|:-----------------------------|:----------------------------|:-------|:-----------------|:---------------------|:---------------------|:--------------------------------------------------|
|       216 | Friday, November 28, 2025    | Schroeder                   | 16:32  | Seattle Torrent  | Minnesota Frost      | Seattle Torrent      | https://www.thepwhl.com/en/stats/game-summary/216 |
|       229 | Wednesday, December 17, 2025 | Ahola                       | 16:10  | Seattle Torrent  | Ottawa Charge        | Ottawa Charge        | https://www.thepwhl.com/en/stats/game-summary/229 |
|       234 | Sunday, December 21, 2025    | Schroeder                   | 17:05  | Seattle Torrent  | Boston Fleet         | Seattle Torrent      | https://www.thepwhl.com/en/stats/game-summary/234 |
|       236 | Tuesday, December 23, 2025   | Desbiens                    | 17:26  | Seattle Torrent  | Montréal Victoire    | Montréal Victoire    | https://www.thepwhl.com/en/stats/game-summary/236 |
|       244 | Saturday, January  3, 2026   | Rooney                      | 16:55  | Ottawa Charge    | Minnesota Frost      | Minnesota Frost      | https://www.thepwhl.com/en/stats/game-summary/244 |
|       246 | Saturday, January  3, 2026   | Frankel                     | 18:49  | Boston Fleet     | Vancouver Goldeneyes | Boston Fleet         | https://www.thepwhl.com/en/stats/game-summary/246 |
|       261 | Tuesday, January 20, 2026    | Kirk                        | 18:27  | Seattle Torrent  | Toronto Sceptres     | Toronto Sceptres     | https://www.thepwhl.com/en/stats/game-summary/261 |
|       272 | Friday, February 27, 2026    | Murphy                      | 17:48  | Seattle Torrent  | Toronto Sceptres     | Seattle Torrent      | https://www.thepwhl.com/en/stats/game-summary/272 |
|       278 | Thursday, March  5, 2026     | Osborne                     | 17:97  | New York Sirens  | Boston Fleet         | New York Sirens      | https://www.thepwhl.com/en/stats/game-summary/278 |
|       283 | Wednesday, March 11, 2026    | Levy                        | 18:49  | Seattle Torrent  | Boston Fleet         | Boston Fleet         | https://www.thepwhl.com/en/stats/game-summary/283 |
|       302 | Sunday, March 29, 2026       | Hensley                     | 18:40  | Minnesota Frost  | Boston Fleet         | Minnesota Frost      | https://www.thepwhl.com/en/stats/game-summary/302 |
|       303 | Sunday, March 29, 2026       | Schroeder                   | 18:23  | Seattle Torrent  | Ottawa Charge        | Seattle Torrent      | https://www.thepwhl.com/en/stats/game-summary/303 |
|       320 | Saturday, April 18, 2026     | Campbell                    | 14:54  | Seattle Torrent  | Vancouver Goldeneyes | Vancouver Goldeneyes | https://www.thepwhl.com/en/stats/game-summary/320 |
|       321 | Sunday, April 19, 2026       | Rooney                      | 18:19  | Minnesota Frost  | Toronto Sceptres     | Minnesota Frost      | https://www.thepwhl.com/en/stats/game-summary/321 |
