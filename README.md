📊 Banking Risk Analysis Dashboard (Power BI)
📌 Project Overview

This project focuses on risk analytics in the banking and financial services domain using Power BI. The goal is to understand how customer data can be leveraged to minimize lending risk and support data-driven decision-making while approving or rejecting loan applications.

The dashboard provides insights into loans, deposits, customer engagement, fees, and account distributions, enabling banks to assess applicant profiles and financial exposure effectively 

Banking Report.docx (1)

.

🎯 Problem Statement

Banks face significant risk when lending money to customers without understanding their financial behavior and engagement patterns.
This project aims to:

Develop a basic understanding of risk analytics

Analyze how banking data helps reduce the risk of loan defaults

Support loan approval decisions based on customer profiles 

Banking Report.docx (1)

💡 Solution

An interactive Power BI dashboard was built to analyze:

Customer demographics

Loan and deposit distributions

Engagement duration

Account-wise financial exposure

The dashboard helps stakeholders determine whether an applicant is likely to repay a loan, supporting safer lending decisions 

Banking Report.docx (1)

.

🗂️ Dataset Description

The dataset contains detailed banking and client-level information stored across multiple interrelated tables, connected using primary and foreign keys.

Key Tables:

Banking Relationship

Client–Banking

Gender

Investment Advisor

Period (Date Hierarchy) 

Banking Report.docx (1)

🧹 Data Cleaning & Feature Engineering

Several derived columns were created to enhance analysis:

🔹 Engagement Timeframe

Categorized customers based on how long they have been associated with the bank.

🔹 Engagement Days

Calculated the number of days a customer has been active since joining the bank using:

DATEDIFF(Joined Bank, TODAY(), DAY)

🔹 Income Band

Customers were segmented based on estimated income:

Low: < 100,000

Mid: < 300,000

High: ≥ 300,000

🔹 Processing Fees

Derived based on fee structure:

High → 0.05

Mid → 0.03

Low → 0.01 

Banking Report.docx (1)

🧮 DAX Measures & Calculations

Key DAX functions used include:

SUM

DISTINCTCOUNT

SUMX

SWITCH

DATEDIFF

Example Measures:
Total Clients = DISTINCTCOUNT('Clients - Banking'[Client ID])

Bank Loan = SUM('Clients - Banking'[Bank Loans])

Total Fees =
SUMX(
    'Clients - Banking',
    [Total Loan] * 'Clients - Banking'[Processing Fees]
)
``` :contentReference[oaicite:5]{index=5}

---

## 📈 Key KPIs
The dashboard tracks the following KPIs:

- Total Clients  
- Total Loan  
- Bank Loan  
- Business Lending  
- Total Deposits  
- Total Fees  
- Savings Account Amount  
- Checking Account Amount  
- Credit Card Balance  
- Foreign Currency Account  
- Customer Engagement Length :contentReference[oaicite:6]{index=6}

---

## 📊 Dashboard Pages
The Power BI report contains multiple interactive pages:

### 🏠 Home Dashboard
- High-level overview of all KPIs
- Summary of loans, deposits, and fees

### 📉 Loan Analysis
- Loan distribution by:
  - Income band
  - Gender
  - Nationality
  - Banking relationship
- Credit card and business lending insights

### 💰 Deposit Analysis
- Deposits by:
  - Account type
  - Engagement timeframe
  - Income band
- Savings, checking, and foreign currency analysis

### 📌 Summary Dashboard
- Consolidated financial snapshot of all metrics for quick decision-making :contentReference[oaicite:7]{index=7}

---

## 🏁 Conclusion
This project demonstrates how **Power BI dashboards** can be effectively used in the banking sector to:
- Monitor key financial metrics
- Understand customer behavior
- Reduce lending risk
- Support strategic business decisions :contentReference[oaicite:8]{index=8}

---

## 🚀 Future Enhancements
- Predictive risk scoring for loan default probability
- Advanced segmentation using ML models
- Time-series analysis for trend forecasting
- Integration with real-time banking data pipelines :contentReference[oaicite:9]{index=9}

---

## 🛠️ Tools & Technologies
- **Power BI**
- **DAX**
- **Data Modeling**
- **Data Visualization**
- **Risk Analytics**

---

### ⭐ If you want:
- A **shorter GitHub version**
- A **resume bullet version**
- A **LinkedIn project description**
- A **README with screenshots & badges**

Tell me — I’ll tailor it exactly for placements 🔥
