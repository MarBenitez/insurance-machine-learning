# Insurance Premium Fractioning Prediction

This repository contains a comprehensive data science project focused on predicting which new clients are eligible for free insurance premium fractioning. The project involves extensive exploratory data analysis (EDA), data preprocessing, feature engineering, and the implementation of various machine learning models.


## Introduction

The goal of this project is to build a machine learning model to predict which new clients are eligible for free insurance premium fractioning based on historical payment data, qualitative information, and demographic details.


## Data Description

The project uses three main datasets:
1. **Historical Payments Data**: Series of payment records for insurance premiums, spanning 1 to 60 months.
2. **Qualitative Information**: Various qualitative attributes for the clients.
3. **Demographic Data**: Complete address, postal code, and state within the USA.


## Exploratory Data Analysis (EDA)

EDA was conducted to understand the distributions, relationships, and potential anomalies in the data. Key visualizations include:
- Distribution of variables such as `MONTHS_BALANCE`, `STATUS`, `CNT_CHILDREN`, `AMT_INCOME_TOTAL`, `DAYS_EMPLOYED`, `CNT_FAM_MEMBERS`, etc.
- Correlation matrix to identify relationships between features.
- Box plots to visualize income distribution across different income types.


## Data Preprocessing

The preprocessing steps included:
- Handling missing values.
- Removing outliers.
- Encoding categorical variables using label encoding.
- Generating a target variable based on historical payment status.


## Feature Engineering

Key features were engineered to enhance the predictive power of the model, including aggregating historical payment data and creating new interaction terms.


## Modeling

Several machine learning models were implemented and compared:
- Ridge Classifier
- Logistic Regression
- AdaBoost Classifier
- Gradient Boosting Classifier

The Gradient Boosting Classifier provided the best performance and was further fine-tuned using GridSearchCV.


## Evaluation

The models were evaluated based on various metrics:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**
- **Confusion Matrix**
- **ROC Curve and AUC**


## Conclusion

The Gradient Boosting Classifier achieved the highest accuracy and balanced performance across all metrics, making it the best choice for this prediction task.


## Insights

- The number of days employed and total income are significant predictors of eligibility.
- The correlation matrix revealed that family size and number of children are highly correlated.
- EDA highlighted the importance of addressing outliers and missing values to improve model performance.


## Future Work

Future improvements could include:

- Further tuning of the model hyperparameters.
- Exploration of additional machine learning algorithms.
- Deployment of the model in a production environment.
- Integration of real-time data for continuous model updates.
- Collaboration with domain experts to refine the feature selection process.

