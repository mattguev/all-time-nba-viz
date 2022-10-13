# all-time-nba-viz

These two visualizations are concerned with answering the question of 'Who were the Detroit Pistons' best players of All-Time, and what statistics did they average during their time there?' I chose to measure performance by the number of Player of the Week awards that player won during their time there. This data was scraped from a Kaggle dataset tracking Players of the Week from 1980 to 2020. I filtered that dataset to only feature players from the Detroit Pistons, then grouped players by number of awards. Afterwards, I merged that data with a CSV from Basketball-Reference.com which records career averages for every Pistons player during the time that they played there. From there, I sorted players by their awards in descending order and took the first five, those being: Isiah Thomas, Andre Drummond, Ben Wallace, Grant Hill, and Chauncey Billups.

The bar chart below plots each player's Pistons career average for 4 statistics: points per game, rebounds per game, assists per game, steals per game, and blocks per game. 

![](https://github.com/mattguev/all-time-nba-viz/blob/main/Bar%20Chart.png?raw=True)

This answers the basic question of what numbers they averaged, but with Basketball being a team sport, I wanted to use another visualization which would better highlight the role that each player would likely take within this hypothetical team. I found a solution to this using Plotly's built-in support for radar plots. 

![](https://github.com/mattguev/all-time-nba-viz/blob/main/Radar%20Chart.png?raw=true)

Using the visualization it produces, we see that Isiah Thomas' (6 NBA POTW Awards) competitive advantage in points (19.2 ppg - 2nd), assists (9.3 apg - 1st), and steals (1.9 spg - 1st) would have made him an ideal candidate to be the team's ball-handler--a versatile floor general capable of dictating the flow of games using his arsenal of passing, scoring or crucial defensive stops. By comparison, a player like Andre Drummond averaged only 14.4 points per game but 13.9 rebounds per game (1st), making him the likely 'big-man' of the team--dominating smaller players in the paint, rebounding missed attempts from the team's shooters, and setting up the offense with Thomas during pick-and-rolls.

Given more time, I would try and find a more representative metric for performance across eras other than Player of the Week. Although convenient for the purposes of these visualizations, it is imperfect for several reasons, one of which being that it cannot facilitate cross-era player comparisons. In this sense, it may be better as a metric for constructing the best teams as represented by one player from each era.
