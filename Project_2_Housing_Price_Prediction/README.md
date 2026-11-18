# California Housing Price Prediction

## Project Overview

This project focuses on predicting median house values using the California Housing dataset. It applies regression techniques and feature engineering to understand the relationship between housing characteristics and property prices.

## Dataset

- **Source:** California Housing Dataset
- **Records:** 20,640
- **Features:** 9 original input features
- **Target:** `median_house_value`
- **Missing Values:** 207 entries in `total_bedrooms`

## Technologies Used

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Statsmodels
- Jupyter Notebook

## Project Workflow

1. Data loading and exploration
2. Exploratory Data Analysis (EDA)
3. Missing-value analysis and imputation
4. Correlation analysis and multicollinearity assessment
5. Feature engineering and interaction features
6. Train-test splitting and preprocessing
7. Linear Regression (OLS)
8. Ridge Regression
9. Lasso Regression
10. Hyperparameter tuning using GridSearchCV
11. Model comparison
12. Residual analysis and visualization

## Engineered Features

- `rooms_per_household`
- `bedrooms_per_room`
- `population_per_household`
- `income_age_interaction`

## Model Performance

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| OLS Linear Regression | 49,376.49 | 69,048.19 | 0.6362 |
| Ridge Regression | 49,382.63 | 69,056.22 | 0.6361 |
| Lasso Regression | Add actual result | Add actual result | Add actual result |
| Tuned Ridge | Add actual result | 69,056.22 | Add actual result |
| Tuned Lasso | Add actual result | 69,049.25 | Add actual result |

**Best Performing Model:** OLS Linear Regression

## Evaluation Metrics

- MAE: Measures average absolute prediction error.
- RMSE: Measures prediction error while penalizing larger errors.
- R² Score: Measures the proportion of target variance explained by the model.

## Visualizations

The notebook includes:

- Missing-value heatmap
- Target distribution
- Correlation heatmap
- Feature relationship plots
- Actual vs Predicted plots
- Residual distribution plots
- Regression model comparison charts

## How to Run

1. Clone this repository.
2. Install the required dependencies:

   `pip install pandas numpy matplotlib seaborn scikit-learn statsmodels jupyter`

3. Open the notebook:

   `jupyter notebook notebooks/housing_price_prediction.ipynb`

4. Run all cells sequentially.

## Conclusion

OLS Linear Regression achieved the best test performance among the evaluated models, with an RMSE of 69,048.19 and an R² score of 0.6362.

This project demonstrates practical applications of regression modelling, preprocessing, feature engineering, model evaluation, and hyperparameter optimization.

---

**Internship Project:** Datheon – Real Estate Housing Price Prediction