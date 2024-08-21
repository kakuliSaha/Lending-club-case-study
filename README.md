# Lending Club Case Study

## Table of Contents
- [Overview](#overview)
- [Objectives](#objectives)
- [Data Exploration](#data-exploration)
- [Methodology](#methodology)
- [Analysis](#analysis)
- [Findings](#findings)
- [Technologies](#technologies)
- [Acknowledgments](#acknowledgments)
- [Contributors](#contributors)

## Overview
Lending Club is a financial platform that connects borrowers with investors for personal loans. The company must evaluate loan applications and decide which applicants are likely to repay and which may default. Credit loss occurs when borrowers fail to repay, resulting in a significant financial hit for lenders. The main goal of this case study is to reduce these losses by identifying risky applicants before approval.

## Objectives
The objective is to use Exploratory Data Analysis (EDA) on the provided dataset to identify applicants with a high risk of defaulting. By recognizing these risky borrowers, Lending Club can mitigate potential credit losses and make more informed lending decisions.

## Data Exploration
The dataset contains past loan applicants' data, including whether they defaulted on their loans. The task is to identify patterns that indicate a high likelihood of default. This analysis can help the company take actions such as denying high-risk loans, lowering the loan amount, or increasing interest rates for such applicants.

Key aspects of the dataset include:
- **Loan Status**: This is the primary indicator of whether a borrower has fully paid their loan, defaulted ("Charged-Off"), or is currently making payments ("Current"). For the purposes of this analysis, loans in "Current" status are excluded.
- **Key Variables**: The analysis focuses on loan amounts, borrower demographics (income, home ownership, employment), and credit indicators (DTI, loan grade, term length, etc.).

## Methodology
1. **Data Cleaning**: Remove rows with "Current" loan status and drop columns with excessive missing data or irrelevant information.
2. **Column Formatting**: Convert object columns to appropriate numeric or categorical types, clean up formatting (e.g., percentages), and ensure consistency.
3. **Column Standardization**: Round currency columns to two decimal places and create new columns for better analysis, such as verification status and issue date components.
4. **Outlier and Missing Data Treatment**: Handle outliers and impute or drop missing values.

## Analysis
- **Univariate & Bivariate Analysis**: Analyze individual variables and their relationships with loan default risk.
- **Category Comparisons**: Compare loan approval criteria across demographics, loan terms, and other attributes to identify high-risk categories.
- **Risk Assessment**: Use the cleaned and standardized dataset to evaluate which factors most strongly predict default.

## Findings
Key insights:
- Loan applicants with longer loan terms (60 months) are more likely to default.
- Certain loan grades, particularly F and G, have higher default rates, though they represent a smaller portion of the dataset.
- Income, employment length, and homeownership status significantly influence loan approval decisions.
- Default risk varies by state, with some states showing higher default probabilities despite lower loan volumes.

## Technologies
- Python 3.9.12
- numpy 1.21.5
- pandas 1.4.2
- matplotlib 3.5.1
- seaborn 0.11.2
- Jupyter Notebook 3.3.2
- JupyterLab 6.4.11
- Anaconda 2.1.4

## Acknowledgments
- Insights and methodologies were informed by [Aditya Bhattacharya](https://www.linkedin.com/in/aditya-bhattacharya-b59155b6/) and upGrad's course materials.
- Resources such as [Exploratory Data Analysis by Prasad Patil](https://towardsdatascience.com/exploratory-data-analysis-8fc1cb20fd15) and various technical documentation.

## Contributors
- Kakuli Saha
- Kalyan Nath Somavarapu

