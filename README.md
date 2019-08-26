# EU-Soccer-Leagues-and-Players-Analysis
## Introduction
World Cup is a huge soccer summit every four years. Although I am not a huge soccer fan of
any player or team, I still enjoy watching world cup and buying sport lotteries. This dataset gives me a broad view of teams and players of European Leagues, which is almost 90% of best soccer players around the world. I am interested in investigating these questions listed below that might be helpful for me to make better predictions of next World Cup matches.

## Dataset

This soccer database comes from Kaggle and is well suited for data analysis and machine learning. Itcontains data for soccer matches, players, and teams from several European countries from 2008 to 2016. https://www.kaggle.com/hugomathien/soccer <br>
● The database is stored in a SQLite database. <br>
● I used SQL to access data and look at how the dierent tables relate to each other. <br>

## Summary of Findings

1. What are the most important features to distinguish a star player from a normal player?
I looked at the correlation coefficients and looked at the average values of all features. My analysis shows that a star player must have high potential, fast reaction speed and strong positioning.

_Limitations:_ I have limited understanding of soccer player statistics, so I deleted around 15 columns from the original dataset. If I’ve done more research of all stats, I might be able to have a more accurate conclusion of important features for star players.

2. Do star players make a huge difference to match results? (Cristiano Ronaldo specifically) By comparing all matches Ronaldo played in the dataset and those matches of his team but without him on the feild, I found that Ronaldo only slightly increased the winning rate of his team. (Increase from 82% to 85% for home game and 61% to 66% for away game) However, since the sample size of matches without Ronaldo is small, the result might not be accurate. We need more matches without Ronaldo result to support this conclusion.

_Limitations:_ Ronaldo played almost all matches. For example, he only missed 1 home game in the season 2008/2009. I don’t have enough data points to strongly support my conclusion that matches have similar results with or without him.

3. Are match results related to the sum of overall rating of players? The difference of sum of players’ overall rating has linear relationship with goals difference between the two teams. The correlation coefficient is 0.45, which shows the linear relationship but not super strong.

_Limitations:_ I use the average of overall rating of players for the total rating of a team, rather than a player’s overall rating of that season. I can also do overall rating query of player of the season, but that would be too complicated and I just want a quick analysis here.

