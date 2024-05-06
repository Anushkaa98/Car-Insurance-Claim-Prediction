# Car Insurance Claim Prediction

## Overview
This project focuses on predicting car insurance claims using various machine learning models. The analysis involves data preprocessing, exploratory data analysis (EDA), feature engineering, and model evaluation. The goal is to accurately predict whether a car insurance policyholder will file a claim based on several factors related to the policyholder and the vehicle.

## Dataset
The dataset is sourced from Kaggle and can be found [here](https://www.kaggle.com/datasets/ifteshanajnin/carinsuranceclaimprediction-classification?select=test.csv). It includes two main files:
- `train.csv`: Contains the training data with features and the target variable.
- `test.csv`: Contains the test data without the target variable.

## Data Preprocessing
Data preprocessing steps include handling missing values, encoding categorical variables, feature scaling, and data balancing. Key transformations include:
- Dropping unnecessary columns such as 'policy_id'.
- Encoding categorical features using `LabelEncoder`.
- Handling imbalanced data using `SMOTE`.

## Exploratory Data Analysis (EDA)
EDA involves:
- Visualizing the distribution of claims with pie charts and histograms.
- Analyzing the impact of various features like age of car, policyholder's age, and NCAP ratings on claims.

## Feature Engineering
Feature engineering efforts focus on:
- Extracting new features like 'torque to rpm ratio'.
- Selecting relevant features based on mutual information scores and correlation analysis.

## Model Building and Evaluation
Several models are evaluated:
- Logistic Regression
- Decision Tree
- Random Forest
- K Nearest Neighbors (KNN)
- XGBoost

Each model's performance is assessed based on accuracy, precision, recall, F1-score, and ROC-AUC score. Decision trees, feature importances, and ROC curves are plotted for detailed analysis.

## Results
The analysis shows varying performance across different models with XGBoost achieving the highest accuracy. The project includes detailed visualization of model performance metrics to assist in interpreting the results.

## Conclusion
This project highlights the effectiveness of different machine learning techniques in predicting car insurance claims. The insights gained can help insurance companies tailor their policies and determine premiums based on the likelihood of claims.

## Dependencies
This project requires Python and several libraries which can be installed via pip:
pip install pandas numpy scikit-learn matplotlib seaborn plotly xgboost imbalanced-learn
