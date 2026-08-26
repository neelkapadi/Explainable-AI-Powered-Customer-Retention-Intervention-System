# Explainable-AI Powered Customer Retention & Intervention System


An end-to-end **Machine Learning and Explainable AI** project for predicting telecom customer churn and converting model predictions into **personalized retention recommendations**.

> **Predict → Explain → Segment → Prescribe → Retain**

## 🎯 Project Overview

Customer churn reduces recurring telecom revenue. This project develops an **Explainable AI-Powered Customer Retention & Intervention System** that:

- Predicts customer churn risk using **CatBoost**
- Explains churn drivers using **SHAP**
- Segments customers by churn risk
- Identifies customer-specific root causes
- Recommends personalized retention interventions

## 📊 Key Results

- **100,000 customers**
- **100 features**
- **Overall churn rate: 49.6%**
- **Best model: CatBoost**
- **ROC-AUC: 0.693**
- **Highest-risk decile churn: 77.9%**
- **Lowest-risk decile churn: 19.5%**

## 🔬 Machine Learning Workflow

```text
Customer Data
      ↓
Data Preparation
      ↓
Model Training
      ↓
Model Evaluation
      ↓
CatBoost Churn Prediction
      ↓
SHAP Explainability
      ↓
Customer Risk Segmentation
      ↓
Personalized Recommendations
      ↓
Customer Retention
```

## 🧠 Key Churn Drivers

The analysis identified important factors including:

- Customer lifecycle / tenure (`months`)
- Equipment age (`eqpdays`)
- Change in usage (`change_mou`)
- Monthly usage (`mou_Mean`)
- Recurring charges (`totmrc_Mean`)
- Handset price (`hnd_price`)
- Revenue change (`change_rev`)
- Overage revenue (`ovrrev_Mean`)

## 📈 Risk Segmentation

Customers were ranked using predicted churn probability and divided into ten risk deciles.

| Segment | Actual Churn Rate |
|---|---:|
| Lowest-risk 10% | 19.5% |
| Highest-risk 10% | **77.9%** |

This enables the business to prioritize retention resources toward customers with substantially higher observed churn risk.

## 💡 Prescriptive Retention Framework

The project moves beyond **"Who will churn?"** toward:

```text
WHO?  → Churn Prediction
WHY?  → SHAP Root-Cause Analysis
WHAT? → Personalized Intervention
```

Example interventions:

| Churn Driver | Potential Intervention |
|---|---|
| Aging device | Device upgrade offer |
| Usage decline | Targeted retention outreach |
| High overage charges | Plan optimization |
| High roaming usage | Roaming package |
| Stable, loyal customer | Avoid unnecessary intervention |

## 📊 Project Visuals

### Explainable AI Retention Framework

![Solution Framework](./images/solution_framework.png)

### Exploratory Data Analysis

![EDA Findings](./images/eda_findings.png)

### Machine Learning Workflow

![ML Workflow](./images/ml_workflow.png)

### SHAP Explainability

![SHAP Analysis](./images/shap_analysis.png)

### Customer Risk Segmentation

![Risk Segmentation](./images/risk_segmentation.png)

## 📑 Project Presentation

The complete 15-slide presentation is available here:

**[📥 View / Download Project Presentation](./GCI_FinalAssignment_NeelKapadi.pptx)**

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- CatBoost
- XGBoost
- SHAP
- Matplotlib
- Seaborn
- Google Colab

## 📁 Repository Structure

```text
customer-churn-retention/
│
├── README.md
├── GCI_FinalAssignment_NeelKapadi.pptx
├── GCI_FinalAssignment_NeelKapadi.ipynb
│
├── models/
│   └── catboost.pkl
│
└── images/
    ├── presentation_preview.png
    ├── eda_findings.png
    ├── solution_framework.png
    ├── ml_workflow.png
    ├── shap_analysis.png
    └── risk_segmentation.png
```

## 🚀 Future Enhancements

- Production deployment of the churn prediction model
- Automated recommendation engine
- Integration of quarterly **NPS**
- Customer health scoring using churn risk, NPS, customer value and usage trends
- Continuous monitoring of intervention effectiveness

## 👤 Author

**Neel Manishkumar Kapadi**  
M.Tech | IIT Guwahati
