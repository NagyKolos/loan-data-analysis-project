# Loan-Data-Analysis-Project

Data analysis of loan repayment performance using data cleaning, exploratory analysis, correlation analysis, and regression modeling.

## Project Overview

This project analyzes the factors associated with loan repayment performance using a large-scale loan dataset. The analysis examines how borrower characteristics and loan conditions relate to whether a loan was fully paid or charged off.

The project focuses on five independent variables:

- Annual Income
- Loan Amount
- Interest Rate
- Employment Length
- Loan Term

The dependent variable is **Loan Status**, coded as:
- `1 = Fully Paid`
- `0 = Charged Off`

## Objectives

- Identify factors associated with successful loan repayment
- Examine the relationship between borrower income and repayment status
- Analyze the effect of interest rates and loan terms
- Determine which variables are statistically significant predictors of repayment
- Use statistical analysis to identify patterns in loan performance

## Data Preparation

The dataset was cleaned and transformed before conducting the analysis. The process included:

- Removing records with missing or invalid values
- Removing observations after the dataset's credit-policy cutoff
- Converting categorical variables into numerical/binary variables
- Transforming annual income using a logarithmic transformation
- Applying a logarithmic transformation to loan amount
- Converting employment length into numerical years
- Converting loan term into a binary variable

## Analysis

The project includes:

1. Descriptive statistics
2. Pivot table analysis
3. Correlation analysis
4. Multiple regression analysis
5. Interpretation of coefficients and statistical significance

## Key Findings

### Loan Term

36-month loans had an **89.1% fully-paid rate**, compared with **77.3% for 60-month loans** in the analyzed dataset.

### Interest Rate

Charged-off loans had an average interest rate of **13.90%**, compared with **11.76% for fully paid loans**.

### Regression Results

The regression model produced an **R² of 0.0521**, meaning the selected variables explained approximately 5.21% of the variation in loan repayment status.

The reported regression results found:

| Variable | Coefficient | P-Value | Significant? |
|---|---:|---:|---|
| Annual Income | 0.0579 | 0.000 | Yes |
| Loan Amount | -0.0032 | 0.2458 | No |
| Interest Rate | -1.5828 | 0.000 | Yes |
| Employment Length | -0.0021 | 0.000 | Yes |
| Term | 0.0612 | 0.000 | Yes |

## Tools Used

- Microsoft Excel
- Pivot Tables
- Data Cleaning
- Descriptive Statistics
- Correlation Analysis
- Regression Analysis

## Files

- [Analysis Workbook](loan_repayment_analysis.xlsx)
- [Project Report](loan_repayment_report.pdf)
