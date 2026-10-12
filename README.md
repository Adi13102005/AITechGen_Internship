# Student Performance Prediction System

An end-to-end Machine Learning project developed as part of the AI/ML Internship. This system analyzes student-related academic and lifestyle attributes to predict final exam performance.

## Project Overview

- **Dataset:** `student_data.csv`
- **Target Variable:** `final_score`
- **Model:** Compared Linear Regression, Decision Tree, and Random Forest; best model selected by R² score

## Workflow & Methodology

1. **Data Understanding & Cleaning** — Inspected data types, checked for missing values and duplicates, and handled them (median imputation for missing numeric values, duplicate rows dropped).
2. **Exploratory Data Analysis (EDA)** — Visualized distributions of key features, a correlation heatmap, and relationships between study hours, attendance, previous scores, and final score.
3. **Feature Selection & Encoding** — Selected features based on correlation strength; encoded categorical variables (e.g. extracurricular activity, internet access) using label encoding.
4. **Model Training & Evaluation** — Performed an 80/20 train-test split and trained three regression models.
   - Mean Absolute Error (MAE): 4.34
   - Root Mean Squared Error (RMSE): 5.27
   - R-squared (R²): 0.587
5. **Model Improvement** — Applied 5-fold cross-validation to check the stability of the best model's performance.
6. **Prediction System** — Built a function that takes new student details as input and returns a predicted final score.

## Key Drivers


Previous academic score and study hours show the strongest positive correlation with final performance; attendance and consistent sleep also contribute positively.

## Repository Structure

```
Student_Performance_ML/
├── dataset/
│   └── student_data.csv
├── notebooks/
│   └── Student_Performance_Prediction.ipynb
├── reports/
│   └── PROJECT_REPORT.md
└── README.md
```

## How to Run

1. Clone the repository: `git clone <repo-url>`
2. Open `notebooks/Student_Performance_Prediction.ipynb` in Jupyter Notebook or Google Colab
3. Run all cells in order

## Technologies Used

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Jupyter Notebook
