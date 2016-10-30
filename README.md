# ML-B-Dota-2-Kaggle-Competition
ML@B (Machine Learning at Berkeley) Dota 2 Kaggle Competition (used machine learning/xgboost)

Placed 2nd in the private leaderboard using xgboost.

Challenge: Predict winner of dota2 match

-Raw data consists of heros in game and gold and exp in 5 minute intervals.

What I did:

-One hot encode the heroes

-Create intervals and cummulative sums features

-Parameterization optimization via grid search

-Create separate models for different portions of data (about 10% of the data was missing the gold and exp data)

What I would have done if I had more time:

-More exploratory data analysis

-More time constructing features

-Actually running the entirety of the grid search

-Construct more hero relationships (possibly team 1, team 2 hero pairwises or teammate pairs)
  -It seems that xgboost (random forests) can cover these relationships fairly well and pairs of heroes don't come up to frequently so there runs the risk of overfitting
