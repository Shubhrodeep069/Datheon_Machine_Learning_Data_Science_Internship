# Predictive Customer Churn Classifier

## Project Overview
This project focuses on predicting customer churn using machine learning techniques on the IBM Telco Customer Churn dataset. It implements Random Forest and XGBoost classifiers to identify customers who are likely to discontinue their telecom subscriptions.

The project also addresses class imbalance using SMOTE and evaluates model performance using ROC-AUC and other classification metrics.

## Objectives
- Predict customer churn using telecom subscription records.
- Handle imbalanced target classes using SMOTE.
- Encode categorical variables using OneHotEncoder.
- Train and compare Random Forest and XGBoost classifiers.
- Optimize churn prediction performance using ROC-AUC evaluation.
- Identify important factors influencing customer churn.

## Dataset
- **Source:** IBM Telco Customer Churn Dataset
- **Total Records:** 7,043
- **Total Features:** 20 input features
- **Target Variable:** Churn
- **Classes:** Yes (Churn), No (No Churn)

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- XGBoost
- Jupyter Notebook
- Joblib

## Project Workflow
1. Dataset loading and exploration.
2. Data cleaning and preprocessing.
3. Handling missing values and duplicate records.
4. Exploratory Data Analysis (EDA).
5. Feature selection and train-test splitting.
6. Numerical scaling and categorical encoding.
7. Class balancing using SMOTE.
8. Random Forest model training and evaluation.
9. XGBoost model training and evaluation.
10. Model comparison and feature importance analysis.
11. Saving trained models and evaluation results.

## Model Performance

| Metric | Random Forest | XGBoost |
|---|---:|---:|
| Accuracy | 77.36% | 78.14% |
| Precision | 57.66% | 58.46% |
| Recall | 55.35% | 60.96% |
| F1-Score | 56.48% | 59.69% |
| ROC-AUC | 0.8185 | 0.8342 |

## Best Performing Model
**XGBoost Classifier**

- ROC-AUC Score: 0.8342
- Accuracy: 78.14%
- Precision: 58.46%
- Recall: 60.96%
- F1-Score: 59.69%

XGBoost achieved better performance than Random Forest across all five evaluation metrics.

## Feature Importance
Important features identified by the models include:

- Contract Type (Month-to-month)
- Online Security
- Internet Service (Fiber optic)
- Payment Method (Electronic check)
- Customer Tenure
- Monthly Charges
- Total Charges
- Tech Support

## Key Findings
- The dataset contains an imbalanced churn distribution.
- SMOTE successfully balanced the training dataset.
- Both models achieved ROC-AUC scores above 0.80.
- XGBoost outperformed Random Forest in the evaluated metrics.
- Contract type and online security were particularly important features for XGBoost.

## Project Structure

Datheon_Task_3_Customer_Churn/
│
├── Customer_Churn_Classifier.ipynb
├── Telco-Customer-Churn.csv
├── README.md
├── requirements.txt
│
└── outputs/
    ├── models/
    │   ├── random_forest_model.pkl
    │   ├── xgboost_model.pkl
    │   └── preprocessor.pkl
    │
    ├── plots/
    │   ├── roc_curve_comparison.png
    │   ├── model_comparison.png
    │   ├── random_forest_feature_importance.png
    │   └── xgboost_feature_importance.png
    │
    ├── model_comparison.csv
    ├── random_forest_feature_importance.csv
    └── xgboost_feature_importance.csv


## Conclusion
This project demonstrates how ensemble machine learning techniques can be applied to predict customer churn in the telecommunications industry.

By handling class imbalance with SMOTE and comparing Random Forest with XGBoost, the project achieved a best ROC-AUC score of 0.8342 using XGBoost.

The results highlight the importance of customer contract type, online security, and internet services in predicting customer attrition.

The developed models can help telecom businesses identify potential churn customers and take proactive retention measures.