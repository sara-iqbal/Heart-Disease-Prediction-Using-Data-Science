# Heart Disease Prediction: Explainable AI in Healthcare 🫀

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Scikit--Learn%20%7C%20XGBoost%20%7C%20SHAP-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)

## Project Overview
Cardiovascular disease is a leading cause of death globally. Early detection is crucial for effective treatment. This project aims to build a robust machine learning pipeline to predict the presence of heart disease while prioritizing **model interpretability**.

Unlike standard "black-box" predictions, this solution uses **SHAP (SHapley Additive exPlanations)** to provide clinicians with transparent decision support, explaining *why* a specific prediction was made.

##  Key Features
* **High Performance:** Achieved an **AUC score of 0.92** using XGBoost.
* **Hyperparameter Optimization:** Utilized **Optuna** for automated and efficient hyperparameter tuning.
* **Explainable AI (XAI):** Integrated SHAP values to visualize feature impact and interaction.
* **Feature Engineering:** Created custom metrics, including a specific **CVD Risk Index**.
* **Robust Validation:** 5-Fold Cross-Validation to ensure the model generalizes well to unseen data.

## Tools & Technologies
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn, XGBoost
* **Optimization:** Optuna
* **Interpretability:** SHAP

## Methodology
1.  **Exploratory Data Analysis (EDA):** Analyzed distributions, correlations, and addressed class imbalance.
2.  **Preprocessing:** Handled missing values, scaled numerical features, and encoded categorical variables.
3.  **Feature Engineering:** Developed interaction terms and a custom cardiovascular risk index to enhance predictive power.
4.  **Model Selection:** Benchmarked Logistic Regression, Decision Trees, and XGBoost.
5.  **Tuning:** Used Optuna to find optimal hyperparameters for the XGBoost model.
6.  **Evaluation:** Assessed using ROC-AUC, Precision-Recall, and Confusion Matrix.

## Results
The optimized XGBoost model outperformed baseline models significantly:

| Model | Accuracy | AUC Score |
|-------|----------|-----------|
| Logistic Regression | 85% | 0.88 |
| Decision Tree | 79% | 0.76 |
| **XGBoost (Tuned)** | **91%** | **0.92** |

## Model Interpretability
Using SHAP summary plots, we identified that **Chest Pain Type**, **Thalach (Max Heart Rate)**, and **Oldpeak** were the most significant drivers of prediction.
<img width="355" height="365" alt="image" src="https://github.com/user-attachments/assets/f1a4b6ec-8413-4886-84d9-e3787f5b995a" />


