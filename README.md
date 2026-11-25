# Mutual-Fund-Overview-and-Insights
Analyzed 814 mutual fund schemes using Python, Excel and Power BI to compare returns, risk and expenses and shortlist the Top 30 funds.

## Project Overview

This project focuses on analyzing mutual fund schemes to understand their investment performance, risk levels, fund categories, and fund manager performance.

The objective is to help investors compare mutual funds using important financial parameters and identify suitable investment options through data analysis and interactive Power BI dashboards.

## Business Objectives

- Analyze mutual fund performance across different categories.
- Compare 1-year and 3-year returns.
- Understand Assets Under Management (AUM).
- Evaluate risk using Standard Deviation, Alpha, Beta, and Sharpe Ratio.
- Compare fund managers and Asset Management Companies (AMCs).
- Rank the top 30 mutual fund schemes using a weighted scoring approach.

## Tools & Technologies

- **Python:** Data cleaning, preprocessing, and analysis.
- **Pandas & NumPy:** Data manipulation.
- **Scikit-learn:** MinMaxScaler for normalization.
- **Microsoft Excel:** Data review and ranking export.
- **Power BI:** Interactive dashboard development.

## Dataset Information

- Dataset: `comprehensive_mutual_funds_data.csv`
- Total Mutual Fund Schemes: 814
- Total Columns: 20
- Duplicate Records: 0
- Eligible Records for 3-Year Return Analysis: 793

The dataset contains information about mutual fund categories, fund managers, AUM, returns, expense ratios, risk indicators, and other financial parameters.

## Data Cleaning & Preparation

The following steps were performed using Python:

1. Loaded and explored the original dataset.
2. Checked missing values and duplicate records.
3. Converted hyphen values into missing values (NaN).
4. Identified missing financial parameters.
5. Excluded 21 records with missing 3-year returns from the ranking analysis.
6. Prepared the cleaned dataset for further analysis.

## Analysis & Ranking Methodology

A weighted scoring model was developed to rank mutual fund schemes.

The ranking model considered:

| Parameter | Weight |
|---|---:|
| 3-Year Returns | 45% |
| Expense Ratio | 20% |
| Fund Age | 15% |
| 1-Year Returns | 10% |
| Standard Deviation (Risk) | 10% |

MinMaxScaler was used to normalize the selected parameters before calculating the final weighted scores.

The top 30 mutual fund schemes were selected based on their final scores and exported to Excel for further analysis.

## Power BI Dashboard

The interactive dashboard consists of three pages:

### 1. Overall Overview
- Total Mutual Fund Schemes
- Total AUM
- Average 1-Year Returns
- Average 3-Year Returns
- Average Expense Ratio
- Total Fund Managers
- AUM by Category
- Fund Distribution
- Returns by Category

### 2. Performance & Comparison
- Expense Ratio by Sub-category
- Top 10 AMCs
- SIP vs Lump Sum Comparison
- Fund Manager AUM Comparison
- Fund Ratings Analysis

### 3. Top 30 & Risk Analysis
- Top 30 Ranked Mutual Funds
- Risk vs Return Scatter Chart
- Standard Deviation vs 3-Year Returns
- Category-wise Fund Distribution

## Key Learnings

- Practical experience in financial data analysis.
- Understanding mutual fund performance and risk indicators.
- Applying data cleaning and preprocessing techniques.
- Building a weighted scoring and ranking model.
- Developing interactive Power BI dashboards.
- Converting financial data into meaningful insights.

## Project Files

- `comprehensive_mutual_funds_data.csv` – Original dataset.
- `cleaned_mutual_funds.csv` – Cleaned dataset.
- `ranked_mutual_funds.csv` – Top 30 ranked schemes.
- `Mutual_Fund_Overview_Insights.ipynb` – Python analysis notebook.
- `Mutual_Fund_Overview_Insights.pbix` – Power BI dashboard.

## Conclusion

This project demonstrates how Python, Excel, and Power BI can be used together to analyze mutual fund performance, evaluate investment risks, and rank schemes using a structured scoring methodology.

It provides a practical understanding of financial analytics and data-driven investment comparisons.
