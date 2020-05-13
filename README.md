# NBA Lineup Analysis on Clustered Player Tendencies
#### 2020 MIT Sloan Sports Analytics Conference Research Paper Audience Winner

## Abstract
Basketball has recently been considered more of a “position-less” sport. Most NBA players have skills, styles, and tendencies that cannot be defined by a single traditional position. With NBA player data that accounts for a player’s efficiency, opportunity, and tendencies, we were able to implement unsupervised machine learning techniques to create a framework for how NBA playing styles can be clustered on the court and used for strategic decision making when building rosters and creating lineup rotations. These player clusters are considered new positions, and they give more accurate and detailed insight to what role a player possesses when on the court and how effective he could be in that role. Our unique methods give players a soft assignment for all clusters, that is, a probabilistic weighting onto each of the clusters indicating their likelihood of specific cluster fit. After analyzing the distribution of the various player stats within each new position, we were able to generate a player role for each cluster. 

We present a more specific way to consider player types and positions in the NBA, while providing insight into which combination of player types yield the most effective basketball performance. Our models also contain a predictive component where we can predict the net rating of a potential lineup. As we have recently witnessed a massive change in playing style by most of the NBA, we offer a more accurate approach for analyzing and understand the roles, responsibilities, and combinations of specific groups of players in the NBA.

## Data

### nba_players_clusters.csv
This dataset contains all players that we collected data for, and ran the clutering technique on. There are 5,512 total observations but only 3,608 players received soft cluster memberships (explained why in our paper). Here you can see all the players and their new positions/clusters, as well as all of their player stats that were taken into account in our clustering.

### nba_lineups.csv
This dataset contains all NBA lineups that we used in our 100 bootstrapped random forest models. Each lineup has "summed" soft cluster probabilities across all 9 clusters for the 5 players in each lineup, as well as all neccessary criteria in which we calculated each lineups Bayesian Net Rating (explained in paper).

### nba_pred_frame(1-9).rda
These datasets contain our 3.1 million possible lineups prediction frame that we created and their Bayesian Net Rating predictions calculated by our bootstrapped random forests. 

## Conclusion
Our work offers an alternative way to consider positions and roles in the NBA. We also provide a framework for how these different positions or clusters interactively play together on the court, providing insights to effective and ineffective lineup combinations of players. Please reach out with feedback or ideas about our work.

### Acknowledgements
This project started as a final project of Jonathan & Samuel's summer undergraduate research experience in sport analytics at Carnegie Mellon University in Summer 2019.

### Authors
- **Samuel Kalman**, Purdue University, kalman@purdue.edu
- **Jonathan Bosch**, Syracuse University, jbosch@syr.edu
- **Maksim Horowitz**, Atlanta Hawks
