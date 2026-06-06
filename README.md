# Customer Churn Intelligence

## Overview

Customer retention is one of the most important growth levers for subscription-based businesses. Acquiring a new customer is often significantly more expensive than retaining an existing one.

This project builds a churn prediction system that identifies customers at risk of leaving and helps businesses take proactive retention measures.

Key highlights:

- Exploratory Data Analysis (EDA)
- Data preprocessing & feature engineering
- Class imbalance handling
- Model training & comparison
- Threshold optimization
- Model explainability with SHAP
- Interactive Streamlit deployment

---

## Machine Learning Pipeline

```text
Raw Customer Data
        │
        ▼
Data Cleaning
        │
        ▼
Feature Engineering
        │
        ▼
ColumnTransformer
 ├── Numerical Scaling
 └── One-Hot Encoding
        │
        ▼
Train/Test Split
        │
        ▼
Class Imbalance Handling
        │
        ▼
Model Training
 ├── Logistic Regression
 ├── Random Forest
 └── XGBoost
        │
        ▼
Threshold Optimization
        │
        ▼
SHAP Explainability
        │
        ▼
Streamlit Deployment
```

---

## Business Perspective

Customer churn prediction is valuable only when it drives business decisions.

This solution enables organizations to:

- Identify high-risk customers before churn occurs
- Prioritize retention campaigns efficiently
- Reduce customer acquisition costs
- Improve customer lifetime value (CLV)
- Design targeted offers for vulnerable customer segments

### Key Business Insights

- Customers on month-to-month contracts exhibit the highest churn risk.
- Lower tenure customers are more likely to leave.
- Higher monthly charges correlate with increased churn probability.
- Customers without support-related services show higher churn tendencies.
- Fiber optic customers demonstrate elevated churn rates compared to other service types.

### Recommended Actions

- Incentivize long-term contracts
- Bundle value-added services
- Launch retention campaigns for new customers
- Provide personalized offers to high-risk customer segments

---

## Dataset

**Telco Customer Churn Dataset**

- 7,043 customer records
- 21 input features
- Binary target variable (Churn)

---

## Models Evaluated

| Model | Purpose |
|---------|----------|
| Logistic Regression | Interpretable baseline model |
| Random Forest | Non-linear ensemble model |
| XGBoost | Gradient boosting model optimized for tabular data |

### Performance Summary

| Model | ROC-AUC | F1 Score |
|---------|---------|---------|
| Logistic Regression | 0.86 | 0.64 |
| Random Forest | 0.85 | 0.65 |
| XGBoost | 0.85 | 0.63 |

---

## Explainability

The project incorporates SHAP (SHapley Additive Explanations) to improve model transparency.

SHAP helps:

- Explain individual predictions
- Understand feature impact
- Visualize global feature importance
- Support business decision-making

Top churn drivers identified:

- Contract type
- Customer tenure
- Monthly charges
- Online security
- Tech support
- Internet service type

---

## Tech Stack

| Area | Technology |
|------|------------|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| ML Models | Logistic Regression, Random Forest, XGBoost |
| Explainability | SHAP |
| Visualization | Matplotlib |
| Web App | Streamlit |
| Deployment Assets | Joblib |

---

## Application Features

- Real-time churn prediction
- Probability-based risk assessment
- Interactive user interface
- Automated preprocessing pipeline
- SHAP-powered model interpretation

---


## Conclusion

This project demonstrates how Machine Learning can be leveraged to move beyond prediction and support business strategy.

By combining predictive modeling, explainability, and deployment, the solution delivers a practical framework for customer retention and churn reduction initiatives.
