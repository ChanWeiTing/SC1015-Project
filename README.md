## About
This is a Mini-project for SC1015 which focuses on predicting the success and reception of video games from a game database. For a detailed walkthrough, please view the source code in order from:
1. Data Extraction
2. Exploratory Analysis and Data Visualisation
3. Advanced Visualization
4. Creating Derived Data
5. Linear Regression
6. Decision Tree
7. Random Forest
8. Neural Network



## Contributors
- @Yixuan1012 (Chia Yi Xuan)
- @Stealphe (Chan Wei Ting)
- @LightningJason (Jason Lim Jiasheng)

## Problem Definition
Are we able to predict if a video game is good (user_score above 8.0) based on its relevant metrics?
Which model would provide the most accurate prediction?

## Exploratory Analysis
Univariate Analysis (Violin plot, Histogram, Boxplot)
Bivariate Analysis (Scatterplot, Heatmap)
Multivariate Analysis


## Models Used
Linear Regression
Random Forest (with grid search, adaboost, gradient boost)
Deep learning (artificial neural network)

## Conclusion
- While all predictor variables are not strongly correlated to the response variable of user score, the most important one seems to be critic score. This can mean that critics have some sort of influence over the public’s opinion to a certain extent, or that users and critics are generally looking out for the same few characteristics of video games which make the difference between a good or bad game.
- Linear regression is not a good model as the variables were not strongly linearly correlated.
- We proceeded to use decision trees (User_score >= 8 is classified as 1 while User_score <8 is classified as 0) to predict where User_score is good or bad with reference to the predictor variables. (73% Accuracy with low false positive rate of 8.0%)
- Random forest was done, which caused the classification accuracy to drop to 72%.
- Grid search was done to find optimal hyperparameters which increased accuracy to 75%.
- Adaboosting and gradient boosting was also utilized which showed that random forest with gradient boosting resulted in the best accuracy thus far. (Accuracy 75.8%)
- Neural Network seems to be the most reliable model that we have created to predict the success of a video game (76% accuracy).
- It is possible to predict if a video game will be successful and well received with an acceptable amount of accuracy.

## Lessons learnt
Ensemble learning techniques to enhance random forest model
Deep learning techniques, creating artificial neural networks
Using keras and tensorflow
Collaborating using GitHub

## References
https://www.kaggle.com/datasets/thedevastator/global-video-game-sales-ratings
https://github.com/nicklimmm/movie-analysis
https://pypi.org/project/pandas-profiling/
https://www.datacamp.com/tutorial/random-forests-classifier-python
https://www.projectpro.io/recipes/optimize-hyper-parameters-of-decisiontree-model-using-grid-search-in-python
https://www.freecodecamp.org/news/how-to-build-your-first-neural-network-to-predict-house-prices-with-keras-f8db83049159/
