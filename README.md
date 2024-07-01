# Predicting Singapore Resale Flat Prices

This project focuses on predicting resale prices of flats in Singapore using machine learning models. The dataset used for this analysis can be found in `Data.zip`. The main notebook for the project is `SingaporeResaleFlatPricesPredicting.ipynb`.

## Overview

In this project, we analyze and predict resale flat prices in Singapore based on various features. The dataset is preprocessed, analyzed, and different machine learning models are trained and evaluated to predict resale prices effectively.

## Data

The dataset used for this project (`Data.zip`) contains information about resale flat prices and relevant features.

## Methodology

1. **Data Preprocessing**: Exploratory Data Analysis (EDA), feature engineering, and handling missing values.
   
2. **Modeling**: Training and evaluating different machine learning models for regression.
   
3. **Evaluation**: Assessing model performance using metrics such as R-squared, RMSE, and MAE.

## Model Comparison and Selection

### Model Performance Scores

- **HistGradientBoostingRegressor**:
  - Train Score: 0.9656
  - Test Score: 0.9652

- **LGBMRegressor**:
  - Train Score: 0.9656
  - Test Score: 0.9651

- **XGBRegressor**:
  - Train Score: 0.9792
  - Test Score: 0.9785

### Reasons for Choosing XGBRegressor

1. **Higher Test Score**: The XGBRegressor exhibits the highest test score (0.9785), indicating slightly better performance on unseen data compared to HistGradientBoostingRegressor and LGBMRegressor.

2. **Lower Risk of Overfitting**: Despite having a higher train score (0.9792), the XGBRegressor shows a relatively small train-test gap (0.0007), suggesting potential robustness and lower risk of overfitting compared to HistGradientBoostingRegressor (train-test gap of 0.0004) and LGBMRegressor (train-test gap of 0.0005).

3. **Consistent Performance**: XGBRegressor demonstrates consistent and robust predictive capabilities with competitive scores on both train and test datasets.

4. **Tuning Flexibility**: XGBoost (XGBRegressor) offers extensive hyperparameter tuning options, providing opportunities for further performance enhancement through careful parameter optimization.

5. **Community Support and Adoption**: XGBoost is widely adopted in academia and industry, supported by a large community and extensive resources for ongoing development and support.

### Conclusion

The XGBRegressor is selected as the preferred model for predicting Singapore resale flat prices due to its superior test performance, manageable train-test gap indicating potential robustness, tuning flexibility, and strong community support. These factors collectively make it well-suited for achieving accurate predictions in your modeling task.

