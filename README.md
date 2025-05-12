# 🏦 Bank Loan Health Monitoring & Predictive Insights

An end-to-end **data-driven Excel dashboard project** for evaluating loan performance, borrower risk, economic impact, and fraud patterns through advanced DAX logic, data modeling, and visual storytelling.

---

## 📊 Project Overview

This project builds a **comprehensive Power Pivot & Excel dashboard** that empowers banking or financial institutions to:

- Assess **loan performance metrics**
- Identify **risky borrower behavior**
- Detect potential **frauds or anomalies**
- Analyze **loan quality and disbursement trends** geographically and economically

The dashboard is fully interactive and supports decision-making via dynamic slicers, KPI cards, DAX measures, and relationship-based modeling.

---

## 🚀 Key Features

### ✅ Executive Summary View
- KPI cards for **Disbursed Amount**, **Expected Amount**, **Amount Received**, **Growth %**, **Average DTI**, and **Average Interest Rate**
- Breakdown of loan statuses: **Active**, **Closed**, **Charged Off**
- Interactive slicers: **State**, **Grade**, **Borrower Experience**, and **Term**
- Line chart of **Loan Amount Trends Over Time** (Disbursed vs Expected vs Received)

### ✅ Loan Quality & Risk Overview
- **Loan Risk Flag**, **DTI Flag**, and **Borrower Experience Flag** via DAX
- Line charts: **Funded Loans trend based on repayment efficiency**
- Pie chart: **Borrower Credits Classification**
- Conditional formatting tables for **Risk Factors Based on States**

### ✅ Fraud & Anomaly Detection
- Fraud detection via complex DAX using conditions like:
  - Unusual installment-to-income or loan-to-income ratios
  - Blank or missing employment titles
  - Duplicate borrowers
  - Low total accounts with risk-prone ownership (RENT, NONE, OTHER)
- Visuals:
  - Heat Map: **State Vs Grade analysis based on potential frauds**
  - Bar chart: **Fraud Count by Ownership Type**
  - Table with **Fraud Flag Summary**

### ✅ Economic & Geographic View
- Geo-map showing **State-wise Loan Fraudulent %**
- Line/area chart of **Funded loan trend based on state risk**
- Scatter Chart: **Charge off % by Unemployment Rate w.r.t Funded Loans**
- Stacked bar: **Loan Volume by Region and Ownership Type**

---

## 🔁 External Data Integration & Modeling

The project integrates **external economic data** to enhance analysis:

- **2021 State-wise Unemployment Rate Dataset**  
  - Joined with the main loan table via **State Abbreviation**
  - Relationship built as a **one-to-many** in the Power Pivot model
  - Used to create an `Unemployment Flag` for risk profiling

---

## 🧹 Data Cleaning & Preparation

Data transformations and cleansing steps:

- Removed nulls and handled blank strings for categorical variables
- Created calculated columns for:
  - `Loan Term (in months)`
  - `Expected Total Payment = Installment × Term`
  - `Repayment Efficiency`, `Fraud Flag`, `Underpaid`, `Overpaid` classifications
- Consolidated employment titles and ownership types into flags
- Linked borrower status and risk metrics using logical DAX branching

---

## 📁 File Contents

- **raw_data** – Containing both raw files of bank loan and unemployment rate
- **Bank_Loan_Analysis.xlsx** – Main Excel workbook with Power Pivot model and dashboards
- **README.md** – This documentation
- **Dashboard Images** – Included for GitHub preview (see below)

---

## 🖼️ Dashboard Preview
![Dashboard Overview](/Dashboard.png)

```markdown


📌 Technologies Used
Microsoft Excel (Power Pivot + Power Query)

DAX (Data Analysis Expressions)

Advanced Charting & Slicers

Excel Data Modeling

🔗 Useful Links
🔗 Email ID: sunnykryadav71432@gmail.com
🔗 LinkedIn Profile: [Sunny Kumar Yadav](https://www.linkedin.com/in/sunnykumaryadav)

📣 If you found this project useful or insightful, feel free to ⭐ star the repository and connect with me on LinkedIn!
