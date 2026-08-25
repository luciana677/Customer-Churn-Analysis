## 📊 Customer Churn Analytics

An end-to-end data analytics project investigating customer churn patterns, customer behavior, service usage, contract types, and billing characteristics to identify factors associated with customer retention and churn.

---

📌 Project Type

- Exploratory Data Analysis (EDA)
- Data Cleaning / Wrangling
- Customer Churn Analysis
- Dashboard / Data Visualization
- Business Intelligence
- End-to-End Analytics Project

---
## Table of Contents

1. [Project Overview](#1-project-overview)
2. [Objectives](#2-objectives)
3. [Project Scope & Tools](#3-project-scope--tools)
4. [Repository Structure](#4-repository-structure)
5. [Data Workflow](#5-data-workflow)
6. [Dataset Overview](#6-dataset-overview)
7. [Analysis & Metrics](#7-analysis--metrics)
8. [Key Insights](#8-key-insights)
9. [Business Recommendations](#9-business-recommendations)
10. [Assumptions & Limitations](#10-assumptions--limitations)
11. [Future Enhancements](#11-future-enhancements)
12. [Dashboard](#12-dashboard)
13. [Deliverables](#13-deliverables)
14. [Author](#14-author)

---

1. Project Overview

Context

Customer retention is an important business concern for subscription-based companies. Understanding why customers leave can help organizations identify high-risk customer segments, improve customer experience, and develop more effective retention strategies.

Problem Statement

The objective of this project was to analyze customer data and identify patterns associated with customer churn. The analysis focuses on customer demographics, tenure, services, contract types, payment methods, and billing characteristics to understand which customer segments are more likely to churn.

Approach

The project involved data inspection, data cleaning, exploratory analysis, and interactive dashboard development.

Key areas investigated include:

- Customer demographics
- Customer tenure
- Internet and phone services
- Contract type
- Payment method
- Monthly charges
- Total charges
- Additional services
- Customer churn

Outcome

The analysis produced a cleaned customer dataset, analytical findings, SQL queries, visualizations, and an interactive dashboard designed to communicate churn patterns and support data-driven customer retention decisions.

---

2. Objectives

Primary Objective

Identify customer characteristics, services, and billing factors associated with customer churn.

Secondary Objectives

- Clean and prepare the customer dataset for analysis.
- Calculate overall customer churn and retention metrics.
- Analyze churn across demographic and service-related segments.
- Investigate the relationship between tenure and churn.
- Examine churn patterns across contract and payment types.
- Analyze monthly and total charges by churn status.
- Develop an interactive dashboard for communicating findings.
- Translate analytical findings into actionable business recommendations.

---

3. Project Scope & Tools

Scope

|Dimension| Details|
|`In Scope`| Customer demographics, services, billing, contracts, tenure, churn behavior and dashboard analysis|
|`Out of Scope`| Individual customer prediction, automated retention campaigns and causal inference|
|`Unit of Analysis`| Individual customer|
|`Target Variable`| "Churn"|
|`Analysis Focus`| Factors associated with customer churn|

Tools & Technologies

|Category| Tool(s) Used|
|----|----|
|`Data Source`| CSV Dataset|
|`Data Processing`| Python|
|`Data Analysis`| Python / Jupyter Notebook|
|`Visualization`| Power BI|
|`Version Control`| Git / GitHub|
|`Documentation`| Markdown|

---

4. Repository Structure
```
📊 Customer-Churn-Analytics
│
├── 📂 data
│   ├── 📂 raw
│   │   └── customer_churn.csv
│   │
│   └── 📂 processed
│       └── customer_churn_cleaned.csv
│
├── 📂 notebooks
│   └── customer_churn_analysis.ipynb
│
│
├── 📂 visuals
│   ├── 📂 dashboard
│   └── customer_churn_dashboard.png
│   |___ customer_churn_dashboard.pbix
│  
│
├── 📄 .gitignore
└── 📄 README.md
```
---

5. Data Workflow
```
Raw Dataset
     ↓
Data Inspection
     ↓
Data Cleaning
     ↓
Exploratory Data Analysis
     ↓
SQL Business Analysis
     ↓
Feature Preparation
     ↓
Power BI Visualization
     ↓
Dashboard & Insights
     ↓
Business Recommendations
```
1. Data Source

The project uses a customer churn dataset containing demographic, service, contract, billing, and churn information.

2. Data Inspection

The dataset was examined for:

- Dataset structure
- Data types
- Missing values
- Duplicate records
- Inconsistent values
- Numerical and categorical variables
- Potential data-quality issues

3. Data Cleaning

Data-quality issues were identified and addressed before analysis.

Particular attention was given to the "TotalCharges" field, where values required cleaning and conversion before numerical analysis.

4. Exploratory Analysis

Customer characteristics were compared across churn groups to identify patterns in customer behavior and service usage.

6. Visualization

Key findings were transformed into interactive Power BI visuals and dashboard components.

7. Output

The final outputs include a cleaned dataset, analytical notebook, SQL analysis, visualizations, and an interactive Power BI dashboard.

---

6. Dataset Overview

Dataset Description

The dataset contains customer-level information covering demographics, services, contracts, billing characteristics, tenure, and churn status.

Key Fields

| Field | Description |
|---|---|
| `customerID` | Unique customer identifier |
| `gender` | Customer gender |
| `SeniorCitizen` | Indicates whether the customer is a senior citizen |
| `Partner` | Whether the customer has a partner |
| `Dependents` | Whether the customer has dependents |
| `tenure` | Number of months the customer has stayed with the company |
| `PhoneService` | Whether the customer has phone service |
| `MultipleLines` | Multiple phone line subscription status |
| `InternetService` | Type of internet service |
| `OnlineSecurity` | Online security subscription |
| `OnlineBackup` | Online backup subscription |
| `DeviceProtection` | Device protection subscription |
| `TechSupport` | Technical support subscription |
| `StreamingTV` | Streaming TV subscription |
| `StreamingMovies` | Streaming movies subscription |
| `Contract` | Customer contract type |
| `PaperlessBilling` | Paperless billing status |
| `PaymentMethod` | Customer payment method |
| `MonthlyCharges` | Monthly amount charged |
| `TotalCharges` | Total amount charged |
| `Churn` | Customer churn status |
Unit of Analysis

One row represents an individual customer.

Target Variable

"Churn"

- "Yes" — Customer churned
- "No" — Customer remained with the company

---

7. Analysis & Metrics

Analytical Approach

The analysis focused on understanding who churns, what services they use, how long they stay, and how billing and contract characteristics relate to churn.

The following areas were investigated:

- Overall churn distribution
- Churn rate
- Customer tenure
- Gender
- Senior citizen status
- Partner and dependent status
- Phone service
- Internet service
- Online security
- Online backup
- Device protection
- Technical support
- Streaming services
- Contract type
- Paperless billing
- Payment method
- Monthly charges
- Total charges

Key Metrics

|Metric| Definition| Purpose|
|----|----|----|
|`Total Customers`| Number of unique customers| Understand customer base size|
|`Churned Customers`| Number of customers who churned| Measure customer loss|
|`Churn Rate`| Churned customers ÷ total customers| Measure overall churn|
|`Retention Rate`| Retained customers ÷ total customers| Measure customer retention|
|`Average Tenure`| Mean customer tenure| Compare customer longevity|
|`Average Monthly Charges`| Mean monthly charges| Examine billing patterns|
|`Average Total Charges`| Mean total charges| Examine customer revenue contribution|


---

8. Key Insights

Insight 1 — Overall Churn

The analysis established the overall distribution of customers who churned versus those who remained with the company, providing a baseline for evaluating customer retention.

Insight 2 — Internet Service

Internet service type showed meaningful differences in churn behavior.

The analysis found a higher churn rate among customers using Fiber optic service compared with customers using DSL and customers without internet service.

Internet Service| Churn Rate
DSL| 18.96%
Fiber optic| 41.89%
No internet service| 7.40%

This makes internet service an important segment for further investigation.

Insight 3 — Contract Type

Contract structure showed an important relationship with customer retention. Customers on shorter-term arrangements demonstrated greater churn risk compared with customers on longer-term contracts.

Insight 4 — Customer Tenure

Customer tenure was an important indicator of retention behavior. Customers with shorter relationships with the company were more likely to churn, while longer-tenured customers generally showed stronger retention.

Insight 5 — Billing

Monthly charges showed differences between churned and retained customers, indicating that pricing and monthly customer cost may be relevant factors in churn analysis.

Insight 6 — Customer Services

Additional services such as online security, online backup, device protection, and technical support were investigated to determine whether service engagement was associated with customer retention.

---

9. Business Recommendations

|Priority| Recommendation| Based On|
|---|---|---|
|`High`| Develop targeted retention strategies for high-churn customer segments.| Segment-level churn analysis|
|`High`| Investigate the factors contributing to the high churn rate among Fiber optic customers.| Internet service analysis|
|`High`| Encourage suitable customers to move toward longer-term contracts through appropriate incentives.| Contract analysis|
|`Medium`| Strengthen early-stage customer engagement to reduce churn among newer customers.| Tenure analysis|
|`Medium`| Review pricing and billing patterns among high-churn customers.| Monthly charges analysis|
|`Medium`| Evaluate the value of additional support and security services as retention tools.| Service-level analysis|

«These recommendations are based on observed associations in the dataset and should be validated with additional business and customer-level information before implementation.»

---

10. Assumptions & Limitations

Assumptions

- Each row represents one unique customer.
- "Churn" is treated as the outcome variable provided in the dataset.
- Customer and service categories are interpreted according to the dataset definitions.
- The analysis focuses on associations rather than causal relationships.

Limitations

- The dataset represents a specific customer population and may not generalize to every telecommunications business.
- Churn analysis identifies patterns but does not establish causation.
- Customer satisfaction, complaints, competitor activity, and other external factors are not included.
- The analysis does not predict individual customer churn.
- Some variables may contain data-quality issues that can influence analytical results.
- Business recommendations should be validated against additional operational and customer feedback data.

---

11. Future Enhancements

Future improvements could include:

- Build a customer churn prediction model.
- Develop customer-level churn risk scoring.
- Perform statistical testing of important churn relationships.
- Conduct deeper customer segmentation.
- Analyze customer lifetime value.
- Investigate the relationship between services and retention.
- Build automated SQL reporting.
- Develop a more advanced Power BI dashboard with drill-through analysis.
- Incorporate additional customer satisfaction and support data.

---

12. Dashboard

Power BI Dashboard

The interactive Power BI dashboard provides an overview of customer churn and allows users to explore churn patterns across customer demographics, services, contracts, tenure, and billing characteristics.

Dashboard Features

- Total customer KPI
- Churned customer KPI
- Churn rate KPI
- Retention rate KPI
- Customer churn distribution
- Churn by contract type
- Churn by internet service
- Churn by payment method
- Tenure analysis
- Monthly charges analysis
- Customer segmentation
- Interactive filters/slicers
- Key analytical insights

## Dashboard KPIs
| Dashboard Component | Metric |
|---|---|
| `Total Customers` | 7,043 |
| `Churned Customers` | 1,869 |
| `Churn Rate` | 26.54% |
| `Average Monthly Charges` | $64.76 |

"Customer Churn Dashboard"

visuals/dashboard/customer_churn_dashboard.png


---

13. Deliverables

|Deliverable| Description| Location|
|---|---|---|
|`Cleaned Dataset`| Processed dataset used for analysis| "/data/processed/"|
|`Jupyter Notebook`| Data cleaning and exploratory analysis| "/notebooks/"|
|`Dashboard`| Interactive Power BI dashboard| Power BI link|
|`Dashboard Screenshot`| Portfolio-ready dashboard image| "/visuals/"|
|`README`| Project documentation| "/README.md"|

---

14. Author

Luciana

Data Analyst | Data Analytics & Business Intelligence

- 🔗 LinkedIn: linkedin.com/in/lucianaidogwu
- 💼 GitHub: https://github.com/luciana677
- 📧 Email: idogwuogechi@gmail.com

---

Last updated: August 2026
