# churn_modeling_project
ML. The goal of this project is to predict customer churn for a retail bank dataset.
# Customer Churn Modeling (Classification)

## Project Overview
This project focuses on predicting customer churn for a retail bank using supervised machine learning.
Customer churn prediction is a classic **imbalanced classification problem**, where missing a churned customer
can be more costly than incorrectly flagging a non-churn customer.

The goal is not only to build accurate models, but also to evaluate them using **churn-relevant metrics**
and provide an interpretable, business-oriented conclusion.

---

## Dataset
The project uses the **Churn_Modelling.csv** dataset (originally from Kaggle):

🔗 https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling/data

**Target variable:**
- `Exited = 1` → customer churned (left the bank)
- `Exited = 0` → customer stayed

The dataset contains **10,000 customers** with demographic, financial, and behavioral attributes.

---

## Project Structure
The notebook follows a structured and transparent machine learning workflow:

1. **Data loading and inspection**
2. **Feature selection and preprocessing**
   - Encoding categorical variables
   - Feature scaling
3. **Exploratory Data Analysis (EDA)**
   - Churn rate analysis
   - Categorical and numerical feature distributions
4. **Model training**
   - Logistic Regression
   - Random Forest
   - Support Vector Machine (SVM)
   - K-Nearest Neighbors (KNN)
   - Gradient Boosting
5. **Handling class imbalance**
   - Class weights
   - Sample weighting
6. **Model evaluation**
   - Precision, Recall, F1-score (for churn class)
   - ROC-AUC and PR-AUC
7. **Threshold analysis for Gradient Boosting**
8. **Final model selection and interpretation**

---

## Evaluation Metrics
Since churn prediction is an imbalanced classification task, **accuracy is not used as the primary metric**.

Instead, we focus on:
- **Recall (class 1)** – ability to identify churned customers
- **Precision (class 1)** – reliability of churn predictions
- **F1-score (class 1)** – balance between precision and recall
- **ROC-AUC** – overall ranking performance
- **PR-AUC** – performance on the positive (churn) class

---

## Final Model
**Gradient Boosting** was selected as the final model because:
- It provid
