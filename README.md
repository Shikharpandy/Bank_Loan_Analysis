# 📊 Bank Loan Analysis Report (SQL + Excel Dashboard)

This project provides a **complete analysis of a bank’s loan portfolio** using **SQL for data cleaning + KPI calculations** and **Excel for dashboard creation and visualization**.
The objective is to evaluate **loan performance, borrower behaviour, repayment trends, and Good vs Bad Loan quality** to support data-driven lending decisions.

---

## 📁 Project Structure

```
├── SQL Queries/
│   ├── Data Cleaning.sql
│   ├── KPI Calculations.sql
│   ├── Good vs Bad Loan.sql
│   └── Trend Analysis.sql
├── Excel Dashboard/
│   ├── Summary Dashboard.xlsx
│   ├── Overview Dashboard.xlsx
│   └── Detailed View.xlsx
├── README.md
```

---

## 🎯 Project Objectives

* Analyse the overall lending activity.
* Track Month-to-Date (MTD) and Month-over-Month (MoM) performance.
* Evaluate borrower risk through **Good vs Bad Loan segmentation**.
* Understand trends in applications, funded amounts, and repayments.
* Build a clear, interactive Excel dashboard for business insights.

---

# 🛠️ Tools & Skills Used

### **SQL**

* Data Cleaning
* Filtering & Aggregation
* Joins & Subqueries
* KPI Calculations (MTD, MoM)
* Good vs Bad Loan Classification

### **Excel**

* Pivot Tables
* Pivot Charts
* Slicers
* Conditional Formatting
* Dashboard Design

---

# 📊 Dashboards & Insights

## **📌 Dashboard 1: Summary**

A high-level view of all key loan metrics:



### **Key KPIs**

* **Total Loan Applications**
* **Total Funded Amount**
* **Total Amount Received**
* **Average Interest Rate**
* **Average Debt-to-Income Ratio (DTI)**

### **Time-Based Metrics**

* Month-to-Date (MTD)
* Month-over-Month (MoM)

### **Good vs Bad Loan Analysis**

**Good Loans** (Fully Paid, Current):

* Good Loan Application %
* Good Funded Amount
* Total Received Amount

**Bad Loans** (Charged Off):

* Bad Loan Application %
* Bad Funded Amount
* Bad Received Amount

### **Loan Status Grid**

Includes:

* Applications
* Funded Amount
* Amount Received
* Avg Interest Rate
* Avg DTI
  <img width="1122" height="566" alt="Screenshot 2025-11-20 210448" src="https://github.com/user-attachments/assets/c67c1d19-8fc3-4136-b43e-1b919ea455ad" />


---

## **📌 Dashboard 2: Overview**

A visual breakdown of loan performance:



* **📈 Monthly Trend Line Charts**
  (Applications, Funded Amount, Amount Received)

* **📊 Loan Term Analysis (Donut Chart)**
  (36 months, 60 months)

* **📉 Employment Length Analysis (Bar Chart)**
  (1 yr, 5 yrs, 10+ yrs)

* **📊 Loan Purpose Analysis (Bar Chart)**
  (Debt Consolidation, Credit Card, etc.)

* **🗂️ Home Ownership Overview (Tree Map Alt.)**
  (Own, Rent, Mortgage)
  <img width="1391" height="669" alt="Screenshot 2025-11-20 210406" src="https://github.com/user-attachments/assets/5bb43a59-dd83-4ba4-ab05-374937b60e47" />


---

## **📌 Dashboard 3: Detailed View**

A fully filterable sheet to explore:

* Borrower details
* Loan features
* State-level information
* Loan purpose
* Loan term
* Home ownership
* Employment length
* Repayment data

This acts as a **master data view** for deep analytics.

---

# 📈 SQL Features Implemented

### ✔ **KPI Calculations**

* Total Applications
* Total Funded Amount
* Total Amount Received
* Avg Interest Rate
* Avg DTI

### ✔ **Time-Based Calculations**

* MTD Applications
* MoM Growth %

### ✔ **Good vs Bad Loan Classification**

```sql
CASE
   WHEN loan_status IN ('Fully Paid', 'Current') THEN 'Good Loan'
   WHEN loan_status = 'Charged Off' THEN 'Bad Loan'
END AS loan_quality
```

### ✔ **Trend Analysis**

Using SQL date functions to extract monthly performance.

---

# 📚 Key Insights Delivered

* Identified which states contribute most to lending volume.
* Highlighted borrowers with higher risk (Bad Loan segment).
* Found peak months for applications and funded amounts.
* Pinpointed loan purposes with highest demand.
* Analysed borrower profiles based on employment and home ownership.

---

# 🧠 What I Learned

* Building automated KPI logic using SQL
* Designing clean & interactive Excel dashboards
* Translating business questions into SQL queries
* Loan portfolio and risk analysis concepts

---

# 📎 How to Use This Project

1. Import dataset into your SQL database.
2. Run SQL scripts in `/SQL Queries/`.
3. Load cleaned output into Excel.
4. Use slicers to explore dashboards interactively.
