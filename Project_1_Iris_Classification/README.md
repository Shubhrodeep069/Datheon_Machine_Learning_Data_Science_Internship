# Iris Flower Classification

## Project Overview
This project implements supervised machine learning classification using the Iris dataset. Two classification algorithms, Logistic Regression and Decision Tree, are trained and evaluated.

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset
The Iris dataset contains 150 observations, four numerical features, and three flower species:
- Setosa
- Versicolor
- Virginica

## Methodology
1. Dataset loading and exploration
2. Exploratory Data Analysis using Seaborn
3. Feature scaling using StandardScaler
4. Train/test splitting (80:20)
5. Logistic Regression training
6. Decision Tree training
7. Model evaluation and comparison
8. Confusion matrix and decision boundary visualization

## Model Performance

| Metric | Logistic Regression | Decision Tree |
|---|---:|---:|
| Accuracy | 93.33% | 93.33% |
| Precision | 93.33% | 93.33% |
| Recall | 93.33% | 93.33% |
| F1-Score | 93.33% | 93.33% |

## Project Structure

Project_1_Iris_Classification/
├── dataset/
│   └── iris.csv
├── notebooks/
│   └── iris_classification.ipynb
└── README.md

## How to Run
1. Clone or download this repository.
2. Install the required dependencies:
   `pip install pandas numpy matplotlib seaborn scikit-learn jupyter`
3. Open the Jupyter Notebook.
4. Run all cells sequentially.

## Conclusion
Both classification models achieved 93.33% accuracy on the test dataset, demonstrating effective classification performance on the Iris dataset.