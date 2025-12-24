
# FinTech Customer Analytics – Digital Wallet Transactions

## Overview

This project analyzes customer behavior for a digital wallet product using transaction-level data.  
The main objectives are to:
- Understand transaction patterns and monthly revenue trends
- Measure customer retention using cohort analysis
- Segment customers using RFM (Recency, Frequency, Monetary)
- Build a simple churn indicator based on recency

The project is designed as a portfolio piece for business analytics / data analytics internships.

---

## Dataset

The dataset contains digital wallet transactions with fields such as:
- Transaction ID and user ID
- Transaction timestamp
- Transaction amount
- Product or bill category
- Payment method
- Cashback and loyalty-related fields (if available)

File used:
- `data/digital_wallet_transactions.csv`

---
## **Tools and Technologies**

- **Python**: pandas, numpy, matplotlib, scikit-learn

- **Jupyter Notebook**

- **Power BI (web)** or Tableau for dashboarding

- **Git & GitHub** for version control and portfolio
---
## Main Steps

1. **Data loading and cleaning**

- Parse timestamps

- Handle missing values

**2. Exploratory Data Analysis (EDA)**
- Monthly GMV and transaction counts

- Active users per month

**3. Cohort Retention Analysis**
- Define signup date as the first transaction per user

- Build cohort vs. month-offset matrix

**4. RFM Segmentation**

- Compute Recency, Frequency, and Monetary value per customer

- Define a simple churn flag based on Recency > 30 days

**5. Dashboard**

- Visualize KPIs, cohorts, and segments in Power BI / Tableau

---

## Key Insights

- Customer retention drops significantly after the first month, indicating that early-stage churn is the primary challenge for the product.
- A relatively small group of high-value customers (high Monetary and Frequency) contributes a disproportionate share of total GMV.
- Customers with high Recency (no transactions in the last 30+ days) show a much higher likelihood of churn.
- Most transactions are low-value and frequent, suggesting the digital wallet is primarily used for everyday payments rather than large purchases.

---

## Repository Structure

```text
.
├─ data/
│  ├─ digital_wallet_transactions.csv
│  ├─ monthly_summary.csv
│  ├─ cohort_retention.csv
│  └─ rfm_customers.csv
├─ notebooks/
│  └─ FinTech_Customer_Analytics.ipynb
├─ dashboard/
│  └─ (Power BI / Tableau exports and screenshots)
├─ reports/
│  └─ (executive summary or PDF report)
└─ README.md

---

