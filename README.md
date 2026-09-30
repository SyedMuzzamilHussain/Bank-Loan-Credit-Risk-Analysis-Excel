# Bank Loan Portfolio & Credit Risk Analysis

An Excel-based data analysis project focused on analyzing a
**self-generated synthetic bank loan portfolio** and exploring loan
performance, customer financial characteristics, loan status, and
credit-risk indicators.

> **Important:** The dataset used in this project is synthetic and
> self-generated for educational and portfolio purposes. It does not
> contain real customer or bank data.

------------------------------------------------------------------------

## Project Overview

This project demonstrates an end-to-end **Microsoft Excel data analysis
workflow** using a synthetic portfolio of **500 loan records** covering
the period **2023--2025**.

The analysis transforms loan-level data into:

-   Portfolio KPIs
-   Loan purpose analysis
-   Employment-type analysis
-   Regional analysis
-   Credit-score risk segmentation
-   Debt-to-income risk segmentation
-   Loan-status analysis
-   Monthly loan-volume analysis
-   PivotTable summaries
-   Dashboard visualizations

------------------------------------------------------------------------

## Business Problem

Banks manage loan portfolios containing customers with different income
levels, credit scores, debt-to-income ratios, loan amounts, employment
types, purposes, and repayment statuses.

The purpose of this project is to demonstrate how Excel can be used to
organize this information, calculate meaningful portfolio metrics,
identify patterns in default indicators, and present the results through
an interactive-style dashboard.

------------------------------------------------------------------------

## Project Objectives

-   Analyze the overall structure and size of the loan portfolio.
-   Calculate key portfolio KPIs.
-   Analyze loan distribution by purpose, employment type, and region.
-   Segment loans using credit score and debt-to-income ratio.
-   Examine default patterns across risk segments.
-   Analyze Active, Closed, Overdue, and Defaulted loan statuses.
-   Analyze monthly loan volume and loan amount.
-   Build PivotTables and charts for portfolio analysis.
-   Create a professional Excel dashboard.

------------------------------------------------------------------------

## Dataset

### Dataset Type

**Self-generated synthetic loan portfolio**

### Dataset Size

-   **500 loan records**
-   **14 original fields**
-   **2 derived analysis fields**
-   Analysis period: **2023--2025**

### Original Fields

  Column               Description
  -------------------- ---------------------------------
  `Loan_ID`            Unique identifier for each loan
  `Application_Date`   Loan application date
  `Customer_Age`       Customer age
  `Employment_Type`    Employment category
  `Annual_Income`      Annual customer income
  `Credit_Score`       Customer credit score
  `Loan_Amount`        Loan amount
  `Interest_Rate`      Loan interest rate
  `Loan_Term_Months`   Loan repayment term
  `Loan_Purpose`       Purpose of the loan
  `Debt_to_Income`     Customer debt-to-income ratio
  `Region`             Geographic region
  `Loan_Status`        Current loan status
  `Default_Flag`       Binary default indicator: 0/1

### Derived Fields

  Column                Description
  --------------------- ------------------------------
  `Credit_Score_Band`   Credit score risk category
  `DTI_Band`            Debt-to-income risk category

------------------------------------------------------------------------

## Data Preparation

The workbook uses separate layers for source data and analysis.

### Workbook Structure

``` text
Raw Data
   ↓
Working Data
   ↓
Analysis
   ↓
PivotTables
   ↓
Dashboard
```

### Data Quality Checks

The project includes checks for:

-   Duplicate Loan IDs
-   Missing values
-   Numeric ranges
-   Categorical values
-   Default flag values
-   Valid application dates
-   Employment categories
-   Loan purposes
-   Regions
-   Loan statuses

The prepared dataset contains **500 valid loan records**.

------------------------------------------------------------------------

## Risk Segmentation

### Credit Score Bands

  Credit Score   Band
  -------------- -----------
  Below 580      Poor
  580--669       Fair
  670--739       Good
  740+           Excellent

### DTI Bands

  DTI         Band
  ----------- --------
  Below 20%   Low
  20%--39%    Medium
  40%+        High

These categories are used to compare default indicators across different
risk segments.

------------------------------------------------------------------------

## Default Methodology

The `Default_Flag` was generated using a **synthetic rule-based random
process**.

The generation logic gives a higher synthetic default probability when
selected characteristics such as:

-   Lower credit score
-   Higher debt-to-income ratio
-   Higher loan amount

meet predefined conditions.

This logic is used only to create realistic-looking synthetic data. It
is **not a validated credit-risk model** and should not be used for real
lending decisions.

------------------------------------------------------------------------

## Key Portfolio Metrics

The final dataset contains:

  Metric                                Value
  --------------------------- ---------------
  Total Loans                             500
  Total Loan Amount             ₹50,98,68,608
  Approx. Total Loan Amount      ₹50.99 crore
  Defaulted Records                       148
  Synthetic Default Rate                29.6%
  Analysis Period                  2023--2025

------------------------------------------------------------------------

## Analysis Performed

### 1. Portfolio KPIs

Calculated metrics include:

-   Total Loan Amount
-   Total Number of Loans
-   Average Loan Amount
-   Average Interest Rate
-   Average Credit Score
-   Average Annual Income
-   Average Debt-to-Income Ratio
-   Default Rate
-   Defaulted Loans
-   Active Loans
-   Closed Loans
-   Overdue Loans

### 2. Loan Purpose Analysis

Analyzed:

-   Number of loans
-   Total loan amount
-   Defaulted loans
-   Default rate
-   Average loan amount

across:

-   Home
-   Education
-   Medical
-   Business
-   Vehicle
-   Personal

### 3. Employment Analysis

Default indicators were analyzed across:

-   Salaried
-   Self-Employed
-   Business

### 4. Regional Analysis

Portfolio and default indicators were analyzed across:

-   North
-   South
-   East
-   West
-   Central

### 5. Credit Score Risk Analysis

Default rates were compared across:

-   Poor
-   Fair
-   Good
-   Excellent

### 6. DTI Risk Analysis

Default rates were compared across:

-   Low
-   Medium
-   High

### 7. Loan Status Analysis

Loan distribution was analyzed across:

-   Active
-   Closed
-   Overdue
-   Defaulted

### 8. Monthly Analysis

Monthly loan volume and total loan amount were analyzed for the 36-month
period from 2023 through 2025.

------------------------------------------------------------------------

## PivotTables

The workbook contains PivotTable analysis for:

-   Loan Status
-   Loan Purpose
-   Employment Type
-   Region
-   Credit Score Band
-   DTI Band
-   Monthly Loan Volume
-   Loan Status & Loan Amount
-   Loan Purpose & Loan Amount
-   Region & Loan Status

Core PivotTable totals were reconciled against the Analysis sheet.

------------------------------------------------------------------------

## Dashboard

The Excel dashboard provides a consolidated view of the portfolio.

### Dashboard KPIs

-   Total Loan Amount
-   Total Loans
-   Average Loan Amount
-   Default Rate
-   Defaulted Loans
-   Active Loans
-   Overdue Loans
-   Closed Loans

### Dashboard Visualizations

-   Loan Status Distribution
-   Loan Volume by Purpose
-   Default Rate by Credit Score Band
-   Default Rate by DTI Band

------------------------------------------------------------------------

## Key Findings

-   The portfolio contains **500 synthetic loan records**.
-   The total loan amount is **₹50,98,68,608**, approximately **₹50.99
    crore**.
-   There are **148 records with `Default_Flag = 1`**, resulting in a
    synthetic default rate of **29.6%**.
-   Monthly analysis covers **36 months** from 2023 through 2025.
-   The project provides multiple dimensions for examining default
    indicators, including credit score, DTI, loan purpose, employment
    type, and region.

------------------------------------------------------------------------

## Business Insights

The analysis demonstrates how portfolio risk can be examined from
multiple perspectives rather than relying on a single overall metric.

Credit score and DTI segmentation provide two different views of
customer risk characteristics. Loan purpose, employment type, and region
provide additional dimensions for understanding portfolio distribution
and potential concentration.

Monthly analysis adds a time-based view that can be used to monitor
changes in loan activity.

Because the dataset is synthetic, these observations describe the
generated dataset and should not be interpreted as real-world banking
conclusions.

------------------------------------------------------------------------

## Recommendations

For a similar real-world analytical environment, the reporting approach
could be extended by:

-   Monitoring default rates by risk segment.
-   Reviewing portfolio concentration by loan purpose, region, and
    employment type.
-   Tracking monthly loan volume and loan amount.
-   Standardizing KPI definitions across reporting periods.
-   Combining descriptive Excel analysis with validated historical data
    and appropriate statistical or machine-learning methods for
    production use.

------------------------------------------------------------------------

## Tools & Skills

### Tools

-   Microsoft Excel

### Excel Skills

-   Data Cleaning
-   Data Validation
-   Data Preparation
-   Excel Formulas
-   `COUNTIF`
-   `SUMIF`
-   `SUMIFS`
-   `COUNTIFS`
-   `AVERAGE`
-   `INDEX`
-   `MATCH`
-   Percentage Calculations
-   PivotTables
-   Charts
-   Dashboard Development
-   Conditional Formatting

### Analytical Skills

-   Exploratory Data Analysis
-   KPI Development
-   Risk Segmentation
-   Portfolio Analysis
-   Business Question Development
-   Business Insights
-   Data Visualization
-   Business Reporting

------------------------------------------------------------------------

## Repository Structure

``` text
Bank-Loan-Credit-Risk-Analysis/
│
├── README.md
│
├── Excel/
│   └── Bank_Loan_Credit_Risk_Analysis_Beautified.xlsx
│
├── Documentation/
│   └── Bank_Loan_Portfolio_Credit_Risk_Analysis_Documentation.docx
│
└── Screenshots/
    └── dashboard.png
```

------------------------------------------------------------------------

## Project Files

### Excel Workbook

The workbook contains:

-   Raw Data
-   Working Data
-   Analysis
-   Dashboard
-   PivotTable analysis sheets

### Documentation

The documentation explains the project methodology, business problem,
objectives, dataset, data dictionary, cleaning, preparation, analysis,
risk methodology, dashboard design, findings, insights, recommendations,
and tools used.

------------------------------------------------------------------------

## Project Limitations

-   The dataset is synthetic and self-generated.
-   Default indicators are generated using predefined synthetic logic.
-   The project is descriptive and does not represent a production
    credit-risk model.
-   The results should not be used for actual customer lending
    decisions.
-   No real customer information or confidential banking information is
    included.

------------------------------------------------------------------------

## Purpose

This project was created as an **Excel data-analysis portfolio project**
to demonstrate practical skills in data preparation, analysis, risk
segmentation, PivotTables, visualization, dashboard creation, and
business reporting.

------------------------------------------------------------------------

## Author

**Syed Muzzamil Hussain**

**Project:** Bank Loan Portfolio & Credit Risk Analysis

**Tool:** Microsoft Excel

**Dataset:** Self-Generated Synthetic Data
