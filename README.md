# Predicting the Next NBA MVP
### Summary
This project focuses on using NBA players' statline to predict the NBA MVPs. Since MVPs are chosen through a process in which a handful of players are rank by sports analysts and broadcaster, the idea is to model the way these individuals cast their votes towards choosing their candidates. In doing so,  determining the next NBA season's MVP will ultimately come down to analyzing specific stats of a player during that season.


### Dataset
The dataset was retrieved from Kaggle that contain players' statlines from 1950s to 2017 NBA season that included regular and advanced stats. In addition, I web scrapped from basketball-reference.com to include the player's team win-lose percentage since I believe this is a huge reason for candidates to win.

Here is the link to the dataset used for this project. https://www.kaggle.com/drgilermo/nba-players-stats


### Approach
The approach to this problem will be to randomly sample 1800 different statlines from the 2000 season till 2017 season. Of this 1800, each season will have 100 statlines where 1 statline will be the definitive MVP for that season and the rest are all non MVPs. The goal is to develop a model using classification algorithms to classify MVPs and non MVPs by hand picking specific features. To determine the definitive MVP for the season, the player with the highest probability output by the model will be considered the definitive MVP.

### Result
The model was able to sucessfully predict the 2018 NBA MVP to be James Harden from the Houston Rocket using Logistic Regression. The feature that had the highest weight was Team's Winning percentage, meaning that most of the focus on how well the team perform throughout the entire season.

![james-harden-reacts-black-uni](https://user-images.githubusercontent.com/35437033/42668823-952c5878-8607-11e8-8990-4f92097404e4.jpg)

### Extension
To get a more objective view on the players, unsupervised learning can be done to help seperate players in hope to finding other trends to discern MVP players. See Capstone Project 1 Final Report for more details.
