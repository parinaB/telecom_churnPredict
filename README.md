# telecom_churnPredict
ML Project: Telecom_Churn
Dataset
The project uses the dataset available online:
https://www.kaggle.com/code/emineyetm/telco-customer-churn
(e.g., Kaggle Telco Customer Churn dataset)

Note: No CSV is included in this repo; analysis is based on the online dataset.

Objective
Predict [target variable, e.g., customer churn] using machine learning and compare the performance of Logistic Regression and Random Forest.

Steps Followed
Data Exploration & Cleaning

Checked missing values and handled them.
Converted categorical variables using encoding.
Explored distributions, correlations, and feature importance.
Feature Engineering

Selected top features based on importance and correlation.
Scaled numeric features using StandardScaler for Logistic Regression.
Model Training & Evaluation

Split data into training and testing sets.
Trained Logistic Regression and Random Forest Classifier.
Evaluated using 5-fold cross-validation and recorded accuracy.
Hyperparameter Tuning

Performed RandomizedSearchCV for Random Forest.
Tuned parameters: n_estimators, max_depth, min_samples_split, min_samples_leaf, max_features.
Observations
Logistic Regression achieved slightly higher accuracy, suggesting the data is mostly linearly separable.
Random Forest is useful for feature importance analysis, even if it doesn’t outperform Logistic Regression.
Tuning Random Forest brought it closer to Logistic Regression, but the difference is minimal.
Model Accuracy
Model	Accuracy (%)
Logistic Regression	80.39
Random Forest (tuned)	80.20
Conclusion
Logistic Regression is simple, interpretable, and performs slightly better for this dataset.
Random Forest helps analyze feature importance and remains competitive after tuning.
This project demonstrates a complete ML workflow: data exploration, preprocessing, model comparison, and hyperparameter tuning, all without storing the dataset locally.
Author
Parina Bhardwaj
