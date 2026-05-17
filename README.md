# 📉 Customer Churn Prediction — End-to-End ML Pipeline

> Predicting telecom customer churn using Python and Random Forest, with a Power BI dashboard for business stakeholders. Achieved **89% classification accuracy** on the Telco Customer Churn dataset.

[![Python](https://img.shields.io/badge/Python-3.10-3776AB?logo=python&logoColor=white)](https://python.org)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3-F7931E?logo=scikitlearn&logoColor=white)](https://scikit-learn.org)
[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 🧩 Problem Statement

Telecom companies lose significant revenue to customer churn. This project builds a **predictive ML pipeline** that identifies high-risk customers before they leave, enabling proactive retention strategies.

**Business Question:** Which customers are most likely to churn — and why?

---

## 🏗️ Project Architecture

```
customer-churn-prediction/
├── churn_prediction.py        # Main ML pipeline
├── WA_Fn-UseC_-Telco-...csv   # Source dataset (7,043 customers)
├── churn_predictions.csv      # Model output with churn probabilities
├── feature_importance.csv     # Top predictors ranked
├── requirements.txt           # Dependencies
├── plots/
│   ├── churn_distribution.png
│   ├── feature_importance.png
│   └── tenure_distribution_by_churn.png
└── README.md
```

---

## 🔬 Approach

| Step | Action |
|---|---|
| Data Cleaning | Handled nulls, encoded categoricals, removed irrelevant columns |
| EDA | Visualized churn rate, tenure patterns, service usage distributions |
| Feature Engineering | Extracted contract type, payment method, service bundle signals |
| Class Balancing | Applied SMOTE to handle 73/27 class imbalance |
| Modeling | Random Forest Classifier (200 estimators, tuned depth) |
| Evaluation | Accuracy, Precision, Recall, F1, Confusion Matrix |
| Output | Exported predictions + feature importance CSVs for Power BI |

---

## 📊 Results

| Metric | Score |
|---|---|
| **Accuracy** | **89%** |
| Precision (Churn) | 84% |
| Recall (Churn) | 79% |
| Top Feature | Contract Type |

---

## 📸 Visualizations

### Churn Distribution
![Churn Distribution](churn_distribution.png)

### Feature Importance — What drives churn?
![Feature Importance](feature_importance.png)

### Tenure by Churn Status
![Tenure Distribution](tenure_distribution_by_churn.png)

---

## ⚙️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/HariharanHarini/customer-churn-prediction.git
cd customer-churn-prediction

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the pipeline
python churn_prediction.py
```

Outputs: `churn_predictions.csv` and `feature_importance.csv` — ready for Power BI import.

---

## 📊 Power BI Dashboard

Open `Dashboard/CustomerChurnDashboard.pbix` (Power BI Desktop required) to explore:
- Overall churn rate KPI
- Churn by contract type, payment method, tenure
- High-risk customer segment breakdown
- Feature importance waterfall chart

---

## 🛠️ Tech Stack

- **Python** — Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, imbalanced-learn
- **SQL Server** — Source data validation and aggregation
- **Power BI** — Business-facing dashboard (DAX, KPI cards, drill-throughs)

---

## 👩‍💻 Author

**Harini Hariharan**
🔗 [LinkedIn](https://www.linkedin.com/in/harinihariharan/) · [GitHub](https://github.com/HariharanHarini) · 📧 harinihariharan0107@gmail.com
