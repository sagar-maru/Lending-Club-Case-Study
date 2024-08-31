# Lending Club Case Study - Overview

## Objective

The goal of this case study is to assist in decision-making for a consumer finance company regarding loan approvals. The aim is to use historical profile data to decide whether to approve or deny a loan based on the applicant's likelihood of repayment.

## Project Description

You work for a consumer finance company that provides various types of loans to urban customers. When a loan application is received, a decision must be made on whether to approve it based on the applicant’s profile. There are two key risks associated with this decision:

1. **Rejection Risk**: If an applicant who would repay the loan is rejected, the company loses potential business.
2. **Default Risk**: If a likely defaulter is approved, it can lead to financial losses for the company.

The dataset contains historical information about past loan applicants and their default status. The objective is to identify patterns that predict default, which can help in making informed decisions such as denying the loan, adjusting the loan amount, or applying higher interest rates to risky applicants.

In this case study, Exploratory Data Analysis (EDA) will be used to understand how different consumer and loan attributes influence the likelihood of default.

## Loan Decision Scenarios

When a loan application is considered, there are two main outcomes:

- **Loan Accepted**: If the loan is approved, it can result in three scenarios:
  - **Fully Paid**: The applicant has paid both the principal and interest fully.
  - **Current**: The applicant is still paying installments and the loan tenure is not complete. These applicants are not classified as 'defaulted'.
  - **Charged-off**: The applicant has not paid installments for an extended period and is classified as having defaulted.

- **Loan Rejected**: If the loan is rejected, there is no transactional history available for those applicants in the dataset, as they do not meet the company's criteria.

## Problem Solving Methodology

1. **Data Understanding**
   - Gain knowledge of the data dictionary.
   - Understand the columns and their domain-specific uses.

2. **Data Cleaning**
   - Remove null-valued columns, columns with a single unique value, and unnecessary columns.
   - Convert data types and handle outliers.
   - Derive new variables as needed.

3. **Univariate Analysis**
   - Analyze each column individually.
   - Plot distributions to gain insights into each variable.

4. **Segmented Univariate Analysis**
   - Analyze data variables by segments to gain deeper insights.

5. **Bivariate Analysis**
   - Explore relationships between two variables to understand their empirical connections.

6. **Recommendations**
   - Provide recommendations on key variables to consider during loan approval.
   - Aim to reduce potential losses for the company.

## Technology Used

- **Python**
- **Pandas**
- **Jupyter Notebook**
- **NumPy**
- **Matplotlib**
- **Seaborn**

This case study will use these technologies to perform detailed analysis and visualization to guide loan approval decisions effectively.

# Lending Club Case Study - Key Summary

## Low Risk Recommendations
- **Prioritize Higher Annual Income**: Accept loans from applicants with higher annual incomes to minimize charge-offs.
- **Opt for 36-Month Terms**: Favor loans with a 36-month term as they show a lower risk of defaults and attract more applicants.
- **Choose Lower Interest Rates**: Prefer loans with interest rates below 7.5% to reduce the likelihood of charge-offs.
- **Focus on Grade A and B Loans**: Accept loans graded A and B, while being cautious with loans graded E, F, and G.

## High Risk Warnings
- **Avoid High Interest Rates**: Loans with interest rates above 13% significantly increase the risk of defaults.
- **Monitor Revolving Line Utilization**: High utilization rates (above 58%) are linked to higher charge-off probabilities.
- **Beware of Long Repayment Terms**: Loans with a 5-year term are associated with increased risk.
- **Be Cautious with Lower Grades**: Avoid loans graded D through G, especially subgrades F5, G3, and G5.
- **Loan Purpose Matters**: Avoid loans for small business, renewable energy, or education, as these are higher risk.
- **Consider Public Records**: Loans to individuals with 1 or 2 derogatory public records or bankruptcy records are riskier.
- **Be Wary of Low-Income Borrowers**: Those with annual incomes between $0 and $20,000 show higher default rates.

## Combined Risk Factors
- **High Loan Amounts with High Interest for Low-Income Groups**: Combining high loan amounts and high interest rates with low incomes increases risk.
- **High Installments with Long Terms**: Combining high installments with long repayment terms heightens risk.
- **Consider Home Ownership and Loan Purpose**: Risk varies based on home ownership status and the loan purpose (e.g., car loans, moving expenses, or small business).
- **State of Residence**: Risk levels can vary by the borrower's state of residence.
- **Income and Loan Purpose**: The combination of income level and loan purpose impacts risk.

These suggestions aim to help Lending Club in making more informed and strategic decisions to manage loan risks effectively.

