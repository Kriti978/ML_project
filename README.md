Project Overview

This project predicts and classifies child malnutrition metrics — stunting, wasting, and underweight — for children under 5 years of age.
It uses machine learning regression and classification models to estimate percentage values and categorize nutritional status based on WHO standards and z-scores.
Feature importance is analyzed using SHAP for better model interpretability.

Dataset

File: datafile.csv

Targets:

Children under 5 years who are stunted (height-for-age) (%)

Children under 5 years who are wasted (weight-for-height) (%)

Children under 5 years who are underweight (weight-for-age) (%)

Data includes health, demographic, and nutrition-related features.

Features & Workflow

Data Cleaning & Preprocessing

Handle missing values (median imputation)

Convert numeric columns to proper format

Clean feature names

Apply PCA to retain 95% variance

Regression

Models: RandomForestRegressor, XGBRegressor

Metrics: R², MAE, RMSE

Bias correction applied

Residual analysis with plots

Classification

Convert numeric targets to categories (Low, Medium, High) using z-scores

Data balancing with SMOTEENN

Model: RandomForestClassifier

Metrics: Accuracy, Precision, Recall, F1-score

Explainability

SHAP used to identify feature importance and influence

Technologies Used

Python 3

Libraries:

pandas, numpy

matplotlib, seaborn

scikit-learn, xgboost

imbalanced-learn (SMOTEENN)

shap

Installation & Setup

Clone the repository:

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name


Install dependencies:

pip install -r requirements.txt


Place datafile.csv in the project folder.

Run the notebook:

jupyter notebook ML_project.ipynb

Results

Regression: Accurate prediction after bias correction

Classification: High accuracy in malnutrition severity classification

SHAP analysis: Key features influencing predictions identified

Future Work

Add more datasets for better generalization

Hyperparameter tuning for optimization

Deploy model as a web application (Flask/Streamlit)

Authors
Kriti Jangra , Muskan Goel
kritijangra2006@gmail.com , muskangoel1004@gmail.com

