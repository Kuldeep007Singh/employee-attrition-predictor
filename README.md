# employee-attrition-predictor
# Employee Attrition Predictor

A machine learning project to predict employee attrition using the IBM HR Analytics dataset.
The goal is to help HR teams identify employees who are likely to leave — before they actually do.

## Problem Statement
Employee attrition is costly for companies. This project builds a classification model 
that predicts whether an employee will leave, and identifies the key factors driving that decision.

## Dataset
- **Source:** IBM HR Analytics Dataset (Kaggle)
- **Size:** 1470 records, 35 features
- **Target:** Attrition (Yes/No)

## Tech Stack
- Python, Jupyter/Google Colab
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn, XGBoost, Imbalanced-learn (SMOTE)

## Project Workflow
1. Exploratory Data Analysis (EDA)
2. Data Cleaning and Feature Engineering
3. Encoding categorical variables
4. Handling class imbalance using SMOTE
5. Model building and comparison
6. Feature importance analysis

## Models Compared
| Model | Class 1 F1 | ROC-AUC |
|---|---|---|
| Logistic Regression | 0.49 | 0.79 |
| Random Forest + SMOTE | 0.24 | 0.73 |
| XGBoost + SMOTE | 0.41 | 0.79 |

**Best Model: Logistic Regression**

## Key Findings
- **Overtime** is the single strongest predictor of attrition
- Employees who **travel frequently** are at higher risk of leaving
- **Single employees** are more likely to leave than married ones
- Employees **stuck without promotions** show higher attrition tendency
- **Long tenure in current role** and a **stable manager relationship** strongly predict retention

## How to Run
1. Clone this repository
2. Open the notebook in Google Colab or Jupyter
3. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
4. Run all cells in order

## Learnings
This project highlighted the real challenge of imbalanced datasets in ML. 
A simple Logistic Regression outperformed more complex models, demonstrating 
that model complexity does not always equal better performance.
