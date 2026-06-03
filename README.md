# Day 12 — Customer Churn Analysis + SHAP Explainability

## Problem statement
Which customers are most likely to churn — and WHY?
Can we explain predictions to enable targeted, personalised retention?

## Dataset
Telco Customer Churn (Kaggle) · 7,043 customers · 21 features · 26% churn rate

## Model
- Algorithm: Random Forest (200 trees)
- ROC-AUC: 0.84 — strong discrimination
- Churn Recall: 51% · Churn Precision: 67%
- Overall accuracy: 80%
- Top churn drivers: Contract type, Tenure, Monthly charges

## SHAP explainability
- Global SHAP summary shows contract type as the dominant churn driver
- Individual SHAP waterfall explains exactly why each customer is at risk
- Enables personalised retention outreach — not generic campaigns

## Key findings
- Month-to-month contracts have dramatically higher churn than annual
- Churn peaks in first 6 months — onboarding is the critical window
- Online security and tech support services reduce churn when present
- High monthly charge customers churn more — loyalty pricing opportunity

## Financial impact
- Average customer CLV: £2,096
- Annual customers at churn risk: 1,869
- Retained through model-guided intervention: 243 customers
- ANNUAL REVENUE SAVED: £509,365

## Recommendations
1. Target month-to-month high-risk customers with contract upgrade offers
2. Structured 90-day onboarding programme for new customers
3. Bundle security and support services — reduces churn and increases CLV
4. Loyalty pricing for high monthly charge customers at 6-month mark

## Tools
Python · Random Forest · SHAP · Scikit-learn · Matplotlib · VS Code
