# Football-Dataset

Most and least valuable player

Objective:-The data provided had various attributes given for different players for different seasons and we had to evaluate the players based on a calculated metric.
Steps followed

1.	Analyzed the data and found that each player had many rows with different attributes, to reduce ambiguity I aggregated the row by grouping the rows on player_id and took mean for all variable attributes and mode for all categorical variables
2.	After this I had each row dedicated to a single player
3.	Then I applied K means clustering on the data and found out 4 clusters were giving the best explanation of the variance in data which also coincided with the case as general segregation in football between players are Goal keeper, Forward , Defense , Mid field.
4.	I analyzed each cluster to find out which cluster belongs to which aforementioned the football player category
5.	Saved the different clusters into separate DataFrames  and named them df_mid, df_att, df_gk, df_def
6.	Then, I prioritized the most important attributes at each playing position for example a forward needs to have high acceleration, shot power etc.
7.	Calculated overall score for each category of players taking 4 most important attributes for that category of player and giving equal weights for each one.
8.	Saved top and lowest rated players in different dataframes for each position.
