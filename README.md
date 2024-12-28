# Customer-Churn-Prediction-Bank-
A machine learning project to predict customer churn using techniques like SMOTE for class balancing, Logistic Regression, and Decision Trees. Includes data preprocessing, model evaluation, and feature analysis.

# Customer Churn Prediction

## Overview
This project implements a machine learning solution to predict customer churn based on demographic, behavioral, and financial data. The goal is to identify customers likely to leave a subscription-based service, enabling businesses to take proactive measures to improve retention.

The solution leverages techniques such as data preprocessing, class imbalance handling (SMOTE), and model evaluation using advanced metrics like precision, recall, and F1-score.

---

## Project Highlights
- **Dataset**: Bank Customer Churn Prediction Dataset ([Kaggle](https://www.kaggle.com/datasets/shantanudhakadd/bank-customer-churn-prediction))
  - 10,000 customer records with 14 features including `CreditScore`, `Geography`, `Gender`, `Age`, and `Exited` (churn indicator).
  - Highly imbalanced dataset (79.63% retained, 20.37% churned).

- Techniques Applied:
  - Data Preprocessing:
    - Feature scaling (StandardScaler) for numerical features like `CreditScore` and `Balance`.
    - Encoding categorical variables (`Geography`, `Gender`) using label and one-hot encoding.
    - Removal of irrelevant features (`RowNumber`, `CustomerId`, `Surname`).
  - Class Imbalance Handling:
    - Applied SMOTE (Synthetic Minority Oversampling Technique) to balance churned and retained classes in the training set.
  - Modeling:
    - Baseline models: Logistic Regression, Decision Tree.
    - Evaluation metrics: Precision, Recall, F1-Score, Accuracy.



## Model Performance
### Logistic Regression
| Metric        | Retained (0) | Churned (1) |
|---------------|--------------|-------------|
| Precision     | 89%          | 39%         |
| Recall        | 75%          | 64%         |
| F1-Score      | 81%          | 49%         |

- Strengths: High precision for retained customers.
- Weaknesses: Struggles with identifying churned customers due to low precision.

### Decision Tree
| Metric        | Retained (0) | Churned (1) |
|---------------|--------------|-------------|
| Precision     | 88%          | 41%         |
| Recall        | 78%          | 59%         |
|   F1-Score    | 83%          | 48%         |

- Strengths: Slightly better recall for churned customers than Logistic Regression.
- Weaknesses: Still struggles with precision for churned predictions.

---

Tools and Libraries
- Programming Language: Python
- Key Libraries:
  - `pandas` and `numpy`: Data manipulation and analysis.
  - `scikit-learn`: Machine learning models, preprocessing, and evaluation.
  - `imblearn`: SMOTE for class balancing.
  - `matplotlib` and `seaborn`: Data visualization.


