# ML Project: [Your Project Name]

## Dataset
The project uses the dataset available online:  
[Dataset Link]  
*(e.g., Kaggle Telco Customer Churn dataset: https://www.kaggle.com/blastchar/telco-customer-churn)*

> **Note:** No CSV is included in this repo; analysis is based on the online dataset.

## Objective
Predict [target variable, e.g., customer churn] using machine learning and compare the performance of Logistic Regression and Random Forest.

## Steps Followed
1. **Data Exploration & Cleaning**
   - Checked missing values and handled them.
   - Converted categorical variables using encoding.
   - Explored distributions, correlations, and feature importance.

2. **Feature Engineering**
   - Selected top features based on importance and correlation.
   - Scaled numeric features using `StandardScaler` for Logistic Regression.

3. **Model Training & Evaluation**
   - Split data into training and testing sets.
   - Trained **Logistic Regression** and **Random Forest Classifier**.
   - Evaluated using **5-fold cross-validation** and recorded accuracy.

4. **Hyperparameter Tuning**
   - Performed **RandomizedSearchCV** for Random Forest.
   - Tuned parameters: `n_estimators`, `max_depth`, `min_samples_split`, `min_samples_leaf`, `max_features`.

## Observations
- Logistic Regression achieved slightly higher accuracy, suggesting the data is mostly linearly separable.
- Random Forest is useful for feature importance analysis, even if it doesn’t outperform Logistic Regression.
- Tuning Random Forest brought it closer to Logistic Regression, but the difference is minimal.

## Model Accuracy
| Model                  | Accuracy (%) |
|------------------------|-------------|
| Logistic Regression    | 80.39       |
| Random Forest (tuned)  | 80.20       |

## Conclusion
- Logistic Regression is simple, interpretable, and performs slightly better for this dataset.  
- Random Forest helps analyze feature importance and remains competitive after tuning.  
- This project demonstrates a **complete ML workflow**: data exploration, preprocessing, model comparison, and hyperparameter tuning, all without storing the dataset locally.

## Author
**Parina Bhardwaj**  
