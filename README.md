# Bank Customer Churn Prediction – Machine Learning Project

## Project Overview
Beta Bank has observed a gradual increase in customer churn over time. Since retaining existing customers is more cost-effective than acquiring new ones, the bank wants to predict which clients are likely to leave soon.

This project builds a machine learning model to predict customer churn based on historical behavior and account information. The main focus is maximizing the **F1 score**, while also evaluating the **AUC-ROC** metric.

## Objective
The main objectives of this project are to:
- Predict whether a customer will leave the bank.
- Handle class imbalance effectively.
- Train and compare multiple machine learning models.
- Achieve an F1 score of at least **0.59** on the test dataset.
- Evaluate model performance using both F1 and AUC-ROC metrics.

## Dataset
The dataset contains customer-level banking data with the following features:
- Credit score, age, geography, and gender
- Account balance and estimated salary
- Number of products used
- Credit card ownership
- Customer activity status
- Target variable: `Exited` (1 = customer left, 0 = customer stayed)

## Data Preparation
- Removed non-informative identifiers.
- Encoded categorical variables.
- Scaled numerical features where required.
- Split the data into training, validation, and test sets.
- Examined class imbalance in the target variable.

## Baseline Model
- Trained an initial model without addressing class imbalance.
- Evaluated baseline performance using F1 score.
- Observed the impact of imbalance on model quality.

## Handling Class Imbalance
To improve model performance, at least two techniques were applied:
- Class weight adjustment
- Oversampling and/or undersampling techniques

Different models and hyperparameters were tested using training and validation datasets to identify the best-performing approach.

## Model Evaluation
- Selected the best model based on validation F1 score.
- Evaluated final performance on the test dataset.
- Verified that the F1 score met or exceeded **0.59**.
- Calculated and analyzed the AUC-ROC score.
- Compared F1 and AUC-ROC metrics to assess overall model quality.

## Tools Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

## Business Value
This project helps Beta Bank:
- Identify customers at risk of leaving.
- Improve retention strategies through predictive analytics.
- Reduce customer acquisition costs.
- Support decision-making with machine learning insights.

The project demonstrates a complete machine learning pipeline, including preprocessing, handling class imbalance, model selection, evaluation, and business interpretation.

