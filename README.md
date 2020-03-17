# Analysis of Major League Baseball (MLB) Statistics with Supervised Learning Models

_Work by Song Ying and Antoine Ghilissen_

__Executive Summary__: Analyzing Major League Baseball (MLB) World Series statistics (1946-2016) to formulate in-game strategies for maximal chance of winning a match.

Using the dataset compiled by Retrosheet, we achieved the following:
1. Data Exploration
2. Performed Data Cleaning & Feature Engineering
2. Baseline Model via Logistic Regression (ROC-AUC score: 53.14 %)
3. Decision Tree (ROC-AUC score: %)
4. Random Forest (ROC-AUC score: %)
5. XGBoost (ROC-AUC score: %)
6. Variable & Model Selection
7. Threshold Selection (Threshold: )
8. Final Evaluation
9. Actionable Insights

__Data Source__: MLB Game Logs (1871-2016) sourced from Retrosheet. Dataset can be found here: https://data.world/dataquest/mlb-game-logs

__Methodology__: This project uses Python 3, documented with Jupyter Notebook. We used a combination of Numpy and Pandas for data cleaning, filtering and feature engineering. As the initial stage of feature selection, the cleaned data was checked for multicollinearity using correlation matrix, variance inflation factor (VIF) and our business expertise. A train-test split of 70:30 and 5-fold cross validation was employed for all our models. Logistic Regression was used as our baseline model. Subsequent advanced models like Decision Tree, Random Forest and XGBoost were developed to provide feature selection and to improve model performance. GridSearchCV was used for hyperparameter tuning for Decision Trees, Random Forest and XGBoost. Models were compared using the ROC-AUC score. 

__High Level Overview__: The project started by exploring the data and transforming the dataset into a desirable format. As the original dataset was given in match-by-match basis, we divide each match (row) into 2, namely the winning team and losing team with their respective statistics. As a result, we doubled our number of rows but halved the number of columns, additionally we defined our target variable, the match outcome in a boolean format. As the original dataset was given match-by-match, we had no class imbalance issue as we had a perfect 50:50 split of winners and losers. After data cleaning, we did a preliminary round of feature selection based on correlation matrix to remove trivial variables and removed several other variables using variance inflation factor to ensure there were low multicollinearity between the metrics. 

Next, we created a logistic regression model as our baseline model, which obtained an ROC-AUC score of 53.14 %. To improve on our baseline performance, we developed additional models, namely Decision Trees, Random Forest and XGBoost, which performed at __input__, __input__, __input__ respectively after GridSearchCV optimization. As a result, __input__ was chosen as our final model. A threshold of __input__ was chosen for our final model to optimize for both Type 1 and Type 2 errors. Finally, we evaluated the performance of the model and derived actionable insights for our stakeholders, as described in detail below.

__Files__:
- <code>index.ipynb</code> : main Jupyter Notebook
- <code>MLB-GameLogs-1871_2016.csv</code> : Original Dataset csv
- <code>data_cleaning.ipynb</code> : Data Cleaning Jupyter Notebook
- <code>df.csv</code> : Cleaned Dataset csv
- <code>presentation.pdf</code> : Presentation Slides


__Limitations__:
1. Data samples from 1970-1979 and 1990-1999 were missing and therefore not included in our analysis.
2. Missing players individual statistics to evaluate influence on match outcome by individual factors

__Future Work__:
1. In-depth analysis of linescore paired with match statistics per innings of the game from other sources to investigate probability of winning the match as the match progresses.
2. Evaluation of model on other baseball leagues to ensure consistency and scalability of our model
3. Application of dimensionality reduction techniques like Support Vector Machines to the model
4. Application of unsupervised learning model using Principle Component Analysis & Clustering

__Actionable Insights__:
1. 
