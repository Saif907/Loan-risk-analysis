# Bank Loan Risk Analysis & Default Prediction

An end-to-end **Power BI + Machine Learning** solution that delivers portfolio insights and predicts potential loan defaults. This project combines an interactive Power BI dashboard with an **XGBoost classification model** trained to identify high-risk borrowers, enabling data-driven decisions for lending teams.

---

## 📸 Dashboard Previews

### Page 1: Summary  
Executive overview of portfolio performance and risk segmentation.  
![Summary Page](dashboard/Page1.png)

### Page 2: Overview  
In-depth trend and demographic analysis of funded amounts.  
![Overview Page](dashboard/Page2.png)

### Page 3: Details  
Tabular view of individual loan records for drill-down and validation.  
![Details Page](dashboard/Page3.png)

---

## 🤖 Machine Learning Integration

To complement the dashboard, an **XGBoost ML model** was built to predict customer default risk.

- **Target Variable:** Loan default (Charged Off vs. Fully Paid)  
- **Features Used:** Borrower income, DTI, loan grade, loan amount, interest rate, employment length, purpose, and more  
- **Modeling Tools:** Python, scikit-learn, XGBoost

### 📊 Model Evaluation

**Confusion Matrix:**


\[\[9466  178]
\[ 213 1387]]


- **True Negatives (TN):** 9466  
- **False Positives (FP):** 178  
- **False Negatives (FN):** 213  
- **True Positives (TP):** 1387

**Classification Report:**
          precision    recall  f1-score   support
       0       0.98      0.98      0.98      9644
       1       0.89      0.87      0.88      1600

accuracy                           0.97     11244


macro avg       0.93      0.92      0.93     11244
weighted avg       0.96      0.97      0.97     11244



**Interpretation & Business Value**
- **Overall accuracy: 97%** — the model predicts loan status with a high degree of correctness on the test set.  
- **Class 1 (Default) performance:** precision 0.89 and recall 0.87 — strong at identifying actual defaults while keeping false alarms reasonably low.  
- **Operational impact:** helps identify high-risk loans early, supports credit decisioning and collections prioritization, and can reduce expected loan losses when integrated into workflows.

*(Optional)* Consider adding `notebook/feature_importance.png` (a bar chart of top predictors from XGBoost) to the repository for a quick visual of what drives model decisions.

---

## 🔑 Key Takeaways

- **Default Risk Concentration:** 13.8% of loans charged off, concentrated in lower grades (C–E).  
- **Top Predictors:** Borrower income, loan grade, and DTI are among the most important features for predicting defaults.  
- **Behavioral Insight:** Higher DTI (>20%) correlates with elevated default rates.  
- **Seasonality:** Funded amount rises through the year (e.g., ~$25M in Jan → ~$54M in Dec).  
- **Primary Use Cases:** Debt consolidation dominates; secondary uses include credit card payoff and home improvement.

---

## 🛠️ Technical Summary

- **Dashboard Platform:** Power BI Desktop  
- **Data Prep:** Power Query & Excel  
- **ML Model:** XGBoost (Python)  
- **Evaluation:** Train/test split, cross-validation, confusion matrix, precision/recall/F1, AUC-ROC (recommended)  
- **Visuals in Dashboard:** KPI cards, bar/column charts, line charts, maps, donut charts, tables, slicers  
- **Dataset:** Anonymized loan application dataset (~38.6K records)

---

## 📂 Repository Structure



loan-risk-analysis/
├── dashboard/
│   ├── Loan\_Risk\_Analysis.pbix   # Power BI report
│   ├── Page1.png                 # Dashboard preview - Summary
│   ├── Page2.png                 # Dashboard preview - Overview
│   └── Page3.png                 # Dashboard preview - Details
│
└── notebook/
├── LoanRiskAnalysis.ipynb    # ML model training & evaluation (XGBoost)
└── requirements.txt          # Python dependencies (recommended)





## 🚀 Getting Started

### 1) Clone repository
bash
git clone https://github.com/Saif907/loan-risk-analysis.git
cd loan-risk-analysis


### 2) Power BI Dashboard

* Open `dashboard/Loan_Risk_Analysis.pbix` in Power BI Desktop to interact with the report.
* Use slicers, drill-through and export features to explore data and export visuals.

### 3) Machine Learning Notebook

* Navigate to the `notebook/` folder and open `LoanRiskAnalysis.ipynb` in Jupyter or VS Code.
* Install dependencies:

```bash
pip install -r notebook/requirements.txt
```

* Run the notebook to reproduce data preparation, model training, evaluation, and to export model artifacts / feature importance visualizations.

---

## 🎯 Skills Demonstrated

* Data modeling & ETL (Power Query)
* Interactive dashboard design (Power BI)
* Machine Learning model development & evaluation (XGBoost, scikit-learn)
* Risk analysis & KPI design
* Data storytelling for stakeholders

---

## ✅ Tips for Next Steps (optional)

* Expose model predictions in the dashboard by exporting inference results into a table visual (e.g., predicted probability + risk band).
* Add threshold tuning and business-cost analysis (cost of FN vs FP) to choose the optimal decision threshold.
* Build a simple API to serve the model for real-time scoring (Flask/FastAPI + Docker).
* Track model drift and set up periodic re-training.

---

## 🤝 Get in Touch

* **GitHub:** [Saif907](https://github.com/Saif907)
* **LinkedIn:** [Saif Shaikh](https://www.linkedin.com/in/saifshaikh-analytics251)
* **Email:** [saif81868@gmail.com](mailto:saif81868@gmail.com)

---


