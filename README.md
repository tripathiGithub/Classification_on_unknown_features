
# Objective:
We would like to predict that a person X will buy a product Y. There are a bunch of largely demographic related features available about person X. There are also features available around X’s past activities. We also have aggregated data about people who typically buy product Y available as features (their demographics and past activities). We however do not know which features are which with certainty. The variable C tells us if the person X actually bought the product Y

Full Notebook Report : https://github.com/tripathiGithub/Classification_on_unknown_features/blob/main/ML_Classification.ipynb

# Target Distribution
![image](https://github.com/amancrackpot/Classification_on_unknown_features/raw/main/Results/targetDist.png)

### It was an imbalance binary classification problem
- I used 'class_weight' to deal with the imbalance, it allows models to give more weightage to minority class 

# Models Experimented:
- Logistic Regression 
- Random Forest
- LightGBM
- XGboost
- CatBoost

## Metrics Used
- Area Under Precision Recall Curve for choosing the best model and hyper-parameter tuning
- F1-score for threshold tuning

# Model Comparisions:
![image](https://github.com/amancrackpot/Classification_on_unknown_features/raw/main/Results/modelCompare.png)

## Best Model - CatBoost with PR-AUC = 0.42 and F1 score = 0.52 (on validation set)
![image](https://github.com/amancrackpot/Classification_on_unknown_features/raw/main/Results/bestmodel.png)

# Test set Results:
![image](https://github.com/amancrackpot/Classification_on_unknown_features/raw/main/Results/test_set_results.png)
