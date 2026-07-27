I realized that at least 14 `goalie_change` events are missing from the official data, and the TOI for those goalies was not updated accordingly. 
I attempted to manually add these events. Code is in [Pulling_the_goalie.ipynb](Pulling_the_goalie.ipynb)

Watch my [Youtube video](https://www.youtube.com/shorts/5g5ICNt7at0) explanation or [subscribe to my newsletter](https://365hockeygirl.beehiiv.com/subscribe) to read the full analysis! :D

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
