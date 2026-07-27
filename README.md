# PWHL Pulling the Goalie Data!
I realized that at least 14 `goalie_change` events are missing from the official data, and the TOI for those goalies was not updated accordingly. 
I attempted to manually add these events. 

Code is in [Pulling_the_goalie.ipynb](Pulling_the_goalie.ipynb)

Watch my [Youtube video](https://www.youtube.com/shorts/5g5ICNt7at0) explanation or [subscribe to my newsletter](https://365hockeygirl.beehiiv.com/subscribe) to read the full analysis! :D

## Games affected by missing goalie pull events and extra goalie TOI

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
|       278 | Thursday, March  5, 2026     | Osborne                     | 17:27  | New York Sirens  | Boston Fleet         | New York Sirens      | https://www.thepwhl.com/en/stats/game-summary/278 |
|       283 | Wednesday, March 11, 2026    | Levy                        | 18:49  | Seattle Torrent  | Boston Fleet         | Boston Fleet         | https://www.thepwhl.com/en/stats/game-summary/283 |
|       302 | Sunday, March 29, 2026       | Hensley                     | 18:40  | Minnesota Frost  | Boston Fleet         | Minnesota Frost      | https://www.thepwhl.com/en/stats/game-summary/302 |
|       303 | Sunday, March 29, 2026       | Schroeder                   | 18:23  | Seattle Torrent  | Ottawa Charge        | Seattle Torrent      | https://www.thepwhl.com/en/stats/game-summary/303 |
|       320 | Saturday, April 18, 2026     | Campbell                    | 15:10  | Seattle Torrent  | Vancouver Goldeneyes | Vancouver Goldeneyes | https://www.thepwhl.com/en/stats/game-summary/320 |
|       321 | Sunday, April 19, 2026       | Rooney                      | 18:19  | Minnesota Frost  | Toronto Sceptres     | Minnesota Frost      | https://www.thepwhl.com/en/stats/game-summary/321 |

## Adjusted GAA numbers with goalie pull TOI subtracted

| goalie    |   official_gaa |   adjusted_gaa |    gaa_diff | team                 | time_on_ice   |   games_played |   seconds_adjusted |
|:----------|---------------:|---------------:|------------:|:---------------------|:--------------|---------------:|-------------------:|
| Ahola     |        1.92591 |        1.96266 | 0.0367489   | Ottawa Charge        | 124:37        |              2 |                140 |
| Schroeder |        2.55716 |        2.57644 | 0.0192799   | Seattle Torrent      | 1008:56       |             17 |                453 |
| Levy      |        2.32515 |        2.34048 | 0.0153326   | Boston Fleet         | 180:38        |              3 |                 71 |
| Campbell  |        2.16747 |        2.17619 | 0.00871805  | Vancouver Goldeneyes | 719:44        |             13 |                173 |
| Hensley   |        2.68949 |        2.69409 | 0.00460047  | Minnesota Frost      | 780:49        |             13 |                 80 |
| Rooney    |        2.03777 |        2.04204 | 0.0042733   | Minnesota Frost      | 971:39        |             16 |                122 |
| Osborne   |        2.46947 |        2.47347 | 0.0039938   | New York Sirens      | 1579:17       |             27 |                153 |
| Desbiens  |        1.113   |        1.11421 | 0.00120566  | Montréal Victoire    | 1509:26       |             25 |                 98 |
| Murphy    |        2.87432 |        2.87533 | 0.00101282  | Seattle Torrent      | 709:44        |             12 |                 15 |
| Frankel   |        1.17484 |        1.17558 | 0.000742533 | Boston Fleet         | 1583:12       |             26 |                 60 |
| Kirk      |        1.86784 |        1.86803 | 0.000184613 | Toronto Sceptres     | 1349:09       |             23 |                  8 |
