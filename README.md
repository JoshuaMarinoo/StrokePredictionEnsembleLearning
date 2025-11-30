d# Gradient Boosting Ensemble Model — Stroke Prediction
**Contributor:** Joshua Marino  
Part of the project: *Balancing Model Complexity, Accuracy & Sustainability in Healthcare ML*

---

## Overview
This component of the project implements a **Gradient Boosting ensemble model** (XGBoost or LightGBM) to predict stroke risk. The goal is to analyze how a moderately complex model compares to a simple statistical model and a deep learning model in terms of **accuracy, computational cost, and practicality** for healthcare applications.

---

## Dataset
Dataset: **Stroke Prediction Dataset (Kaggle)**  
https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

**Target:** `stroke`  
**Features:** age, gender, hypertension, heart disease, glucose level, BMI, smoking status, etc.

Basic preprocessing includes:
- Handling missing values  
- Encoding categorical variables  
- Addressing class imbalance  
- Train/test split  

---

## Model Description
The ensemble model uses **Gradient Boosting**, which builds many trees sequentially, each improving the errors of the previous ones. It is widely used in real-world tabular ML tasks and typically achieves high accuracy with reasonable computational cost.

**Why Gradient Boosting?**
- Strong performance on structured medical data  
- Captures nonlinear patterns  
- More accurate than Random Forest in most tabular use cases  
- Good balance between complexity and efficiency  

---

## Evaluation
The model is evaluated using:

- **Accuracy**
- **F1-score**
- **ROC-AUC**
- **Confusion Matrix**
- **Training Time** (for computational cost comparison)

These metrics will be compared with the statistical and deep learning models in the final project report.

---

## Team Roles
- **Arden Sentak** — Statistical Model  
- **Isabella Valentino** — Deep Learning Model  
- **Joshua Marino** — Gradient Boosting Ensemble Model 

---

## How to Run

Install dependencies:
```bash
pip install xgboost numpy pandas scikit-learn

