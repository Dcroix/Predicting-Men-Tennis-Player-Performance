# Machine Learning on Men Tennis Dataset

## Scenario
Data Scientists were hired to determine upcoming tennis players who are likely to not progress into the second week of the Grand Slam Tournaments. After being identified, these players could undergo interventions specific to their techniques or tactics needing improvement. Historical data on players' match performances, sourced from University of California Irvine, was utilized to train a machine learning model to address this problem.

Dataset
The data was explored and pre-processed preparing for machine learning modelling. Variables relevant to addressing the problem were considered as explanatory variables for the model which includes the following:

- FNL - Final Number of Games Won
- FSP - First Serve Percentage
- FSW - First Serve Won
- SSP - Second Serve Percentage
- SSW - Second Serve Won
- ACE - Aces Won by Player
- DBF - Double Fault Committed by Player
- BPC - Break Points Created by Player
- BPW - Break Points Won by Player
- NPA - Net Points Attempted
- NPW - Net Points Won
  
These were the variables that had data through out the 4 Tournaments: US Open, Australian Open, French Open, and Wimbledon. Few missing cases on the dataset were addressed using K-Nearest Neighbor Imputation technique. Undersampling was utilized to reduce the imbalance in the train set while ensuring that it still has more observations than the test set. These were done after the 70-30 train-test split to avoid data leakage.

The response variable labeled "C2" refers to the classification of players. It is an engineered feature which includes two levels for classification:

- 1 - These are players who did not make it to the semifinals or played in the quarterfinals and lost.
- 2 - These are players who at least made it to the semifinals.

You can check out the project in this [link](https://github.com/Dcroix/TennisML/blob/main/MLTennis.ipynb)

