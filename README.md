# Mod_5_Project

_Work by Song Ying and Antoine Ghilissen_

__Executive Summary__: Analyzing Major League Baseball (MLB) World Series statistics (1946-2016) to formulate in-game strategies for maximal chance of winning a match.

Using the dataset compiled by Retrosheet, we achieved the following:
1. Data Exploration
2. Performed Data Cleaning & Feature Engineering
2. Baseline Model via Logistic Regression 
3. Decision Tree
4. Random Forest
5. XGBoost
6. Variable & Model Selection
7. Threhold Selection
8. Final Evaluation
9. Actionable Insights

__Data Source__: MLB Game Logs (1871-2016) sourced from Retrosheet. Dataset can be found here: https://data.world/dataquest/mlb-game-logs

__Methodology__: This project uses Python 3, documented with Jupyter Notebook. We used a combination of Numpy and Pandas for data cleaning, filtering and feature engineering. As the initial stage of feature selection, the cleaned data was checked for multicollinearity using correlation matrix, variance inflation factor (VIF) and our business expertise. A train-test split of 70:30 and 5-fold cross validation was employed for all our models. Logistic Regression was used as our baseline model. Subsequent advanced models like Decision Tree, Random Forest and XGBoost were developed to provide feature selection and to improve model performance. GridSearchCV was used for hyperparameter tuning for Decision Tree, Random Forest and XGBoost. Models were compared using the ROC-AUC score. 

__High Level Overview__:

__Files__:
- <code>index.ipynb</code> : main Jupyter Notebook
- <code>MLB-GameLogs-1871_2016.csv</code> : Original Dataset csv
- <code>data_cleaning.ipynb</code> : Data Cleaning Jupyter Notebook
- <code>df.csv</code> : Cleaned Dataset csv

__Limitations__:
1. Data samples from 1970-1979 and 1990-1999 were missing and therefore not included in our analysis.
2. 

__Future Work__:
1. In-depth analysis of linescore paired with match statistics per innings of the game from other sources to investigate probability of winning the match as the match progresses.
2. Evaluation of model on other baseball leagues to ensure consistency and scalability of our model
3. Application of dimensionality reduction techniques like Support Vector Machines to the model
4. Application of unsupervised learning model using Principle Component Analysis & Clustering
5. 

__Actionable Insights__:
1. 
