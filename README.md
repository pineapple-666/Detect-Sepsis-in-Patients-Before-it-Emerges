# Detect-Sepsis-in-Patients-Before-it-Emerges
🩺 Early Detection of Sepsis Using Machine Learning

ADEC/ADAN 7430 Midterm Project – Fall 2025

📖 Project Overview

This project aims to detect sepsis in patients before it emerges using clinical data from the 2019 PhysioNet Computing in Cardiology Challenge. The objective is to build and compare classification models that can identify whether a patient ever had sepsis, based on aggregated vital signs, laboratory values, and demographic data.

I chose the patient-level classification task — transforming the dataset so that each patient corresponds to one observation (patient_id is unique). The target variable (sepsis) equals 1 if the patient ever developed sepsis.

🧩 Key Steps
1. Exploratory Data Analysis (EDA)

Explored feature distributions across vital signs, lab results, and demographics.

Identified and handled missing values through imputation strategies.

Generated summary statistics and visualized correlations to understand feature relationships.

Learned to manage data types and cleaning, ensuring consistency across variables.

2. Data Preprocessing

Aggregated time-series data to patient-level observations.

Addressed class imbalance using SMOTE (Synthetic Minority Oversampling Technique).

Applied stratified splitting to maintain label distribution in train/test sets.

Prevented data leakage by applying SMOTE only to the training data.

3. Model Development

Implemented and compared multiple classification models:

Logistic Regression (baseline, with feature selection and regularization)

Linear Discriminant Analysis (LDA)

Quadratic Discriminant Analysis (QDA)

Naïve Bayes

K-Nearest Neighbors (KNN)

All models were trained and validated using k-fold cross-validation (k=10).

4. Model Evaluation

Models were assessed using:

Confusion Matrix

F1 Score

ROC Curve & AUC

Precision-Recall Curve

Given the class imbalance, F1 score and AUC were prioritized over accuracy.

5. Final Model & Insights

Selected the best-performing model based on validation results.

Retrained using the full training data and evaluated on the held-out test set.

Discussed model interpretability, feature importance, and practical limitations.

💡 Key Learnings

Debugged Python statsmodels errors and fixed them under time pressure before submission.

Strengthened understanding of data cleaning, feature engineering, and class imbalance handling.

Improved skills in data visualization and model interpretation through peer and judge feedback.

Enhanced teamwork and project management skills in a collaborative data science setting.
