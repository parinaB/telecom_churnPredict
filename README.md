# Telecom Churn Prediction
ML Project: Telecom_Churn

## Project Overview
This repository contains a machine learning pipeline to predict customer churn using the Telco Customer Churn dataset. The project focuses on data preprocessing, feature engineering, and a performance comparison between linear and ensemble-based models.

## Dataset
The analysis is based on the Kaggle Telco Customer Churn dataset:
https://www.kaggle.com/code/emineyetm/telco-customer-churn

Note: The raw CSV is not included in this repository; calculations and preprocessing steps are designed for the online dataset structure.

## Objective
* Predict the target variable (Churn) using Machine Learning.
* Compare the performance and interpretability of Logistic Regression vs. Random Forest.
* Identify key features influencing customer retention.

## Workflow

### 1. Data Exploration & Cleaning
* Handled missing values and data type inconsistencies (e.g., TotalCharges).
* Converted categorical variables using encoding techniques.
* Explored feature distributions and correlations to understand underlying patterns.

### 2. Feature Engineering
* Selected top-performing features based on importance and correlation metrics.
* Scaled numeric features using StandardScaler to optimize Logistic Regression performance.

### 3. Model Training & Evaluation
* Split the dataset into training and testing sets (80/20).
* Implemented 5-fold cross-validation to ensure model stability.
* Evaluated models based on accuracy and classification metrics.

### 4. Hyperparameter Tuning
* Optimized the Random Forest Classifier using RandomizedSearchCV.
* Parameters tuned: n_estimators, max_depth, min_samples_split, min_samples_leaf, and max_features.

## Model Performance

| Model | Accuracy (%) |
| :--- | :--- |
| Logistic Regression | 80.39 |
| Random Forest (Tuned) | 80.20 |

## Observations & Conclusion
* **Model Selection:** Logistic Regression achieved slightly higher accuracy, suggesting that the decision boundaries in this dataset are largely linear.
* **Interpretability:** Logistic Regression offers a simple, interpretable approach, while Random Forest provides valuable insights into feature importance.
* **Optimization:** While tuning improved the Random Forest performance, the marginal gains suggest that the linear model remains the most efficient choice for this specific data distribution.

## Author
**Parina Bhardwaj**
Computer Science & Software Development
