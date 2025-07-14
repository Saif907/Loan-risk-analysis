# Bank Loan Risk Analysis Dashboard

![Dashboard Preview](dashboard_preview.png)

---

## Project Overview

A comprehensive, interactive **Power BI** dashboard designed to analyze and assess risk factors in personal loan portfolios. By integrating business intelligence best practices and advanced data visualization techniques, this solution empowers stakeholders to make data-driven lending decisions.

---

## Key Features & Business Impact

- **Risk Segmentation**  
  Categorize loans by status (Fully Paid vs. Charged Off) to surface high-risk segments and prioritize mitigation strategies.

- **Creditworthiness Assessment**  
  Analyze debt-to-income ratios, credit history, and employment tenure to refine borrower credit profiles and enhance approval workflows.

- **Performance Monitoring**  
  Track interest rates, installment payments, and total repayments over time to identify trends and optimize pricing models.

- **Demographic Insights**  
  Visualize geographic distribution and employment sectors to inform targeted marketing and underwriting policies.

- **Interactive Filters & KPIs**  
  Drill down by state, loan grade, employment length, and homeownership status. Monitor key metrics such as default rate, average DTI, and total loan volume in real-time.

---

## Technical Summary

- **Platform:** Power BI Desktop  
- **Data Preparation:** Power Query / Excel  
- **Visual Types:** Bar & column charts, scatter plots, KPI cards, slicers  
- **Data Source:** Anonymized loan application records

---

## Dataset Schema

| Column            | Description                                    |
|-------------------|------------------------------------------------|
| `id`              | Unique loan identifier                         |
| `address_st`      | Borrower’s U.S. state                          |
| `emp_lengt`       | Employment duration (e.g., `< 1 year`, `10+`)  |
| `emp_title`       | Job title                                      |
| `grade`, `sub_grade` | Assigned risk grade (A–G)                  |
| `home_own`        | Homeownership status (Rent, Mortgage, Own)     |
| `loan_statu`      | Loan status (Fully Paid, Charged Off)          |
| `loan_amo`        | Requested loan amount (USD)                    |
| `annual_inc`      | Annual income (USD)                            |
| `int_rate`        | Applied interest rate (%)                      |
| `installmen`      | Monthly installment (USD)                      |
| `dti`             | Debt-to-income ratio (%)                       |
| `total_acc`       | Number of open credit accounts                 |
| `total_payment`   | Total amount repaid to date (USD)              |

---

## Repository Structure

```

loan-risk-analysis/
├── Loan\_Risk\_Analysis.pbix    # Power BI dashboard file
├── dashboard\_preview\.png      # Static preview image
└── README.md                  # Project overview & instructions

````

---

## Getting Started

1. **Clone the repository**  
   ```bash
   git clone https://github.com/your-username/loan-risk-analysis-dashboard.git
   cd loan-risk-analysis
````

2. **Open in Power BI Desktop**
   Launch `Loan_Risk_Analysis.pbix`.
3. **Interact & Customize**
   Use built-in slicers and visuals to explore risk metrics, adjust filters, and export insights for reporting.

---

## Skills Demonstrated

* Data modeling & ETL with Power Query
* Interactive dashboard design
* Risk analysis & KPI development
* Stakeholder-focused storytelling through data

---

## Next Steps

* **Integrate additional data sources** (e.g., payment history, credit bureau)
* **Automate data refresh** via Power BI Service / Azure Data Factory
* **Extend reporting** with paginated/embedded visuals

---

## Contact & Collaboration

I welcome your feedback or collaboration inquiries:

* **GitHub:** [your-username](https://github.com/Saif907)
* **LinkedIn:** [Your Name](https://www.linkedin.com/in/saif-shaikh-527346251)
* **Email:** [your.email@example.com](mailto:saif81868@fmail.com)

---

*© 2025 Your Name. All rights reserved.*

```
```
