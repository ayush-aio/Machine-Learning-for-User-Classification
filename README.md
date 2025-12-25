# Machine Learning for User Classification

## Project Overview
This project focuses on predicting whether a free-plan student will purchase a subscription on an online learning platform. The model is built using student behavioral data such as lecture engagement, course activity, and exam participation.

The project was inspired by a real business use case where the goal was to identify high-probability buyers ahead of a Black Friday marketing campaign and target them with personalized ads.

---

## Business Problem
The dataset is highly imbalanced because most students never purchased a subscription due to a free platform campaign. This makes purchase prediction challenging and realistic, requiring careful preprocessing and model evaluation.

---

## Dataset Description
- Target variable: `purchased` (0 = not purchased, 1 = purchased)
- Predictor variables include:
  - Minutes watched
  - Courses started
  - Practice exams attempted
  - Time spent on exams
  - Student country
- All features represent student behavior during the free-plan period only

---

## Data Preprocessing
- Removed extreme outliers from behavioral features
- Checked and reduced multicollinearity using VIF
- Handled missing country values
- Encoded categorical variables
- Performed stratified train-test split to handle class imbalance

---

## Models Implemented
- Logistic Regression
- K-Nearest Neighbors (GridSearch optimized)
- Support Vector Machine (GridSearch optimized)
- Decision Tree (Cost-complexity pruning)
- Random Forest

---

## Model Evaluation
- Confusion Matrix
- Precision, Recall, F1-Score
- Accuracy comparison across models

---

## Key Insights
- Class imbalance significantly impacts prediction difficulty
- Behavioral engagement metrics are strong predictors of purchase intent
- Ensemble models outperform simpler classifiers
- Recall is a critical metric due to business cost of missing potential buyers

---

## Conclusion
The project demonstrates how machine learning can support marketing and business decision-making by identifying high-value users and improving targeting efficiency.

---

## Tools Used
- Python (Pandas, NumPy, Scikit-learn, Statsmodels)
- Seaborn & Matplotlib
- Jupyter Notebook
