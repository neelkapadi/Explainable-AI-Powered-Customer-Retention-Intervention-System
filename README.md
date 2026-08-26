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

<img width="1441" height="810" alt="solution_framework" src="https://github.com/user-attachments/assets/c94e6ec1-e4cb-4c70-88ce-9a7938b5da80" />

### Exploratory Data Analysis

<img width="1441" height="810" alt="eda_findings" src="https://github.com/user-attachments/assets/387bc991-fe7a-4a78-a676-62d8af86ac30" />

### Machine Learning Workflow

<img width="1441" height="810" alt="ml_workflow" src="https://github.com/user-attachments/assets/c593fb1b-c318-4ea5-96a3-098662e81b25" />

### SHAP Explainability

<img width="1441" height="810" alt="shap_analysis" src="https://github.com/user-attachments/assets/8d41590d-69cf-4361-9fed-017bb57c6bc6" />

### Customer Risk Segmentation

<img width="1441" height="810" alt="risk_segmentation" src="https://github.com/user-attachments/assets/3c41a40a-b8a7-44b5-a293-57ab0708d10f" />

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
