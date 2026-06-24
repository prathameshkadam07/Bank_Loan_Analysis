# 🏦 Bank Loan Analysis Project

## 📊 End-to-End Banking Analytics Solution Using SQL Server & Power BI

<img width="706" height="398" alt="image" src="https://github.com/user-attachments/assets/a32755c1-71b1-4fb0-9a90-8536dcc05e16" />


---

# 📌 Project Overview

The Bank Loan Analysis Project is an end-to-end Business Intelligence solution developed using SQL Server and Power BI to analyze lending performance, customer borrowing behavior, repayment trends, and portfolio quality.

The project transforms raw banking data into actionable business insights through interactive dashboards and advanced SQL analysis.

### Key Objectives

- Monitor loan application trends
- Track funded and received loan amounts
- Analyze loan portfolio performance
- Evaluate borrower risk profiles
- Identify geographical lending patterns
- Assess loan quality using Good vs Bad Loan analysis
- Support strategic lending decisions

---

# 🎯 Business Problem

Financial institutions process thousands of loan applications every month.

Management requires a centralized reporting system to answer key business questions:

- How many loan applications are received?
- What amount has been funded?
- How much money has been recovered?
- What percentage of loans become defaults?
- Which states generate maximum lending activity?
- What are the primary reasons customers seek loans?
- How does employment history impact borrowing behavior?

The goal was to develop a comprehensive reporting solution that provides real-time insights into loan performance and customer behavior.

---

# 🛠 Tools & Technologies

| Tool | Purpose |
|--------|----------|
| MS SQL Server | Database Management |
| SSMS | Query Development |
| Power BI | Dashboard Development |
| Power Query | Data Transformation |
| DAX | KPI Calculations |
| Excel | Data Validation |

---

# 📂 Dataset Overview

The dataset contains borrower and loan-related information including:

## Customer Information

- State
- Home Ownership
- Employment Length
- Loan Purpose

## Loan Information

- Loan Amount
- Funded Amount
- Loan Status
- Interest Rate
- Installment
- Total Payment

## Financial Metrics

- Debt-to-Income Ratio (DTI)
- Interest Rate

## Time Information

- Issue Date
- Monthly Trends

### Dataset Size

**38,576 Loan Applications**

---

# 📊 Dashboard 1: Executive Summary

<img width="706" height="398" alt="image" src="https://github.com/user-attachments/assets/8563d2f5-ade1-4c8b-81b8-92a70de1c5b9" />


## Purpose

The Summary Dashboard provides a high-level overview of lending performance and portfolio quality.

---

## KPI Analysis

### Total Loan Applications

**38.6K Applications**

Represents the total number of loans issued by the bank.

### Total Funded Amount

**$435.8 Million**

Total amount disbursed to borrowers.

### Total Amount Received

**$473.1 Million**

Total amount collected from borrowers including repayments.

### Average Interest Rate

**12.0%**

Average lending interest rate across the portfolio.

### Average DTI

**13.3%**

Average Debt-to-Income Ratio of borrowers.

---

## Good Loan Analysis

### Metrics

| Metric | Value |
|----------|---------|
| Good Loan Percentage | 86.2% |
| Applications | 33.2K |
| Funded Amount | $370.2M |
| Amount Received | $435.8M |

### Business Insight

The majority of loans are classified as:

- Fully Paid
- Current

This indicates a healthy loan portfolio and strong repayment performance.

---

## Bad Loan Analysis

### Metrics

| Metric | Value |
|----------|---------|
| Bad Loan Percentage | 13.8% |
| Applications | 5.3K |
| Funded Amount | $65.5M |
| Amount Received | $37.3M |

### Business Insight

Although bad loans represent a small percentage of total applications, they contribute significantly to portfolio risk.

---

## Loan Status Analysis

### Fully Paid

- Applications: 32,145
- Lowest risk category
- Highest repayment performance

### Current

- Applications: 1,098
- Active loan accounts

### Charged Off

- Applications: 5,333
- Defaulted loans

### Key Insight

The dominance of Fully Paid loans indicates strong portfolio quality and effective credit underwriting.

---

# 📊 Dashboard 2: Portfolio Overview

<img width="707" height="398" alt="image" src="https://github.com/user-attachments/assets/cab9405c-2c05-4215-8592-13f2f605fa86" />


## Purpose

The Overview Dashboard provides multi-dimensional analysis of loan activity.

It enables users to analyze:

- Monthly Trends
- Geographic Distribution
- Loan Terms
- Employment History
- Loan Purpose
- Home Ownership

---

# 📈 Monthly Trend Analysis

## Loan Applications by Month

The line chart shows a steady increase in loan applications throughout the year.

### Key Observations

| Month | Applications |
|----------|----------|
| January | 2.3K |
| March | 2.6K |
| June | 3.2K |
| September | 3.5K |
| December | 4.3K |

### Business Insight

Loan demand consistently increased throughout the year.

December recorded the highest application volume.

### Recommendation

Increase operational capacity during peak lending months.

---

# 🌎 Regional Analysis

## Loan Applications by State

The Filled Map visual highlights lending activity across the United States.

### Top Performing States

- California
- New York
- Florida
- Texas

### Business Insight

California generated the highest:

- Loan Applications
- Funded Amount
- Repayment Amount

### Recommendation

Focus marketing campaigns on high-performing regions.

---

# ⏳ Loan Term Analysis

## Distribution by Loan Term

| Term | Applications |
|----------|----------|
| 36 Months | 28K |
| 60 Months | 10K |

### Business Insight

Approximately 73% of borrowers selected 36-month loans.

Customers generally prefer shorter repayment periods.

---

# 👨‍💼 Employment Length Analysis

## Applications by Employment Length

Top category:

### 10+ Years Employment

Applications: **8.9K**

### Business Insight

Borrowers with longer employment histories are more likely to apply for loans and generally represent lower lending risk.

---

# 🎯 Loan Purpose Analysis

## Top Loan Purposes

| Purpose | Applications |
|------------|-------------|
| Debt Consolidation | 18K |
| Credit Card | 5K |
| Other | 4K |
| Home Improvement | 3K |
| Major Purchase | 2K |

### Business Insight

Debt Consolidation is the most common borrowing reason, accounting for nearly half of all applications.

---

# 🏠 Home Ownership Analysis

## Application Distribution

| Home Ownership | Applications |
|-----------------|-------------|
| Rent | 18K |
| Mortgage | 17K |
| Own | 3K |

### Business Insight

Renters represent the largest borrower segment and provide significant lending opportunities.

---

# 📊 Dashboard 3: Loan Details Dashboard

<img width="706" height="395" alt="image" src="https://github.com/user-attachments/assets/f3a05bc4-b93c-4b2d-82b2-73ac50d7a07d" />


## Purpose

The Details Dashboard provides transaction-level visibility into every loan record.

---

## Available Fields

- Loan ID
- Purpose
- Home Ownership
- Grade
- Sub Grade
- Issue Date
- Funded Amount
- Interest Rate
- Installment
- Total Amount Received

---

## Business Benefits

### Loan Monitoring

Allows analysts to investigate individual loan records.

### Risk Assessment

Identifies:

- High-risk loans
- High-interest loans
- Default-prone borrowers

### Audit Support

Provides detailed historical loan information for compliance and reporting purposes.

---

# 💻 SQL Analysis

SQL Server was used to create all KPIs and business metrics.

## SQL Functions Used

```sql
COUNT()
SUM()
AVG()
DATENAME()
MONTH()
GROUP BY
ORDER BY
CAST()
CTE
PARTITION
```

## Analytical Queries Developed

### KPI Queries

- Total Applications
- Funded Amount
- Amount Received
- Interest Rate
- DTI

### Risk Analysis Queries

- Good Loan Percentage
- Bad Loan Percentage
- Loan Status Analysis

### Trend Analysis Queries

- Monthly Trends
- State Analysis
- Loan Purpose Analysis
- Employment Length Analysis
- Home Ownership Analysis

---

# 💡 Key Business Insights

## Insight 1

86.2% of loans are Good Loans, demonstrating strong portfolio health.

## Insight 2

Debt Consolidation is the primary reason customers seek loans.

## Insight 3

California contributes the highest lending activity.

## Insight 4

Customers with 10+ years employment history represent the largest borrower group.

## Insight 5

36-month loans are significantly more popular than 60-month loans.

## Insight 6

Renters form the largest borrower segment.

---

# 🚀 Recommendations

## Recommendation 1

Strengthen risk assessment for Charged-Off loans.

## Recommendation 2

Develop specialized Debt Consolidation lending products.

## Recommendation 3

Increase marketing efforts in California and New York.

## Recommendation 4

Create loyalty programs for long-term employed customers.

## Recommendation 5

Design targeted financial solutions for renters.

---

# 📈 Project Outcome

The Bank Loan Analysis Project successfully delivered:

✅ Loan Portfolio Monitoring

✅ Borrower Segmentation

✅ Risk Assessment

✅ Geographic Analysis

✅ Trend Analysis

✅ Executive Reporting

✅ Interactive Business Intelligence Dashboards

---

# 👨‍💻 Author

## Prathamesh Kadam

### Data Analyst

**Skills Demonstrated**

- SQL Server
- Power BI
- Power Query
- DAX
- Data Cleaning
- Data Modeling
- Business Intelligence
- Data Visualization
- Dashboard Development
- Data Storytelling

---

## ⭐ If you found this project useful, consider giving it a star and connecting with me on LinkedIn.
