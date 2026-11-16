# Credit Risk Insights: What Drives Loan Approval Decisions?

A data analytics project that explores which applicant characteristics most influence whether a loan is approved, using Python, MySQL, Excel and Power BI.

![Python](https://img.shields.io/badge/Python-3.x-blue) ![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458) ![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

---

## Table of Contents
1. [Problem Statement](#problem-statement)
2. [Dataset](#dataset)
3. [Tools & Technologies](#tools--technologies)
4. [Project Workflow](#project-workflow)
5. [Key Insights](#key-insights)
6. [Visualizations](#visualizations)
7. [Recommendations](#recommendations)
8. [Repository Structure](#repository-structure)
9. [How to Run](#how-to-run)
10. [Author](#author)

---

## Problem Statement
Lenders must decide quickly and fairly who qualifies for a loan. This project asks:

> **Which applicant factors (credit score, income, employment status, dependents and existing loans) most influence loan approval, and how can a lender use these patterns to assess risk?**

## Dataset
- **Source:** Kaggle (Loan Approval dataset)
- **File:** `loanapproval.csv` (original, unmodified)
- **Size:** 1,000 records, 11 columns

| Column | Description |
|---|---|
| `applicant_id` | Unique applicant identifier |
| `age` | Applicant age |
| `gender` | Male / Female |
| `marital_status` | Marital status of the applicant |
| `annual_income` | Yearly income |
| `loan_amount` | Loan amount requested |
| `credit_score` | Credit score of the applicant |
| `num_dependents` | Number of dependents |
| `existing_loans_count` | Number of existing loans |
| `employment_status` | Employed / Self-employed / Unemployed |
| `loan_approved` | Target: 1 = approved, 0 = rejected |

## Tools & Technologies
- **Python:** pandas, NumPy, matplotlib, seaborn (Google Colab / Jupyter)
- **MySQL:** querying and aggregating the data
- **Excel:** quick checks and pivot summaries
- **Power BI:** interactive dashboard

## Project Workflow
1. **Data loading & overview:** shape, data types, summary statistics
2. **Data cleaning:** missing values, duplicates, data types, outliers, consistency checks
3. **Feature engineering:** loan-to-income ratio, age group, credit score band
4. **Exploratory data analysis:** distributions, relationships, approval rates by group
5. **Visualization:** 10+ charts
6. **Insights & recommendations**

## Key Insights
> Add or update these once your own analysis is complete.

- About **73%** of applicants in the dataset were approved.
- **Credit score** shows the strongest positive link with approval: approval is roughly 57% for scores up to 600 and roughly 92% above 600.
- **Unemployed** applicants have a much lower approval rate (about 51%) than employed (about 82%) and self-employed (about 85%) applicants.
- More **dependents** and more **existing loans** are both associated with lower approval.
- Approval rates for male and female applicants are very close, so gender does not appear to drive decisions in this data.

## Visualizations
> Add screenshots here, for example:

```
![Approval by credit score band](images/approval_by_credit_band.png)
![Approval by employment status](images/approval_by_employment.png)
```

## Recommendations
- Use credit score bands as a first screening layer for risk.
- Look more closely at applicants with several existing loans or dependents when assessing repayment capacity.
- Consider income and loan-to-income ratio together, not income alone.

## Repository Structure
```
├── data/
│   └── loanapproval.csv
├── notebooks/
│   └── loan_approval_analysis.ipynb
├── sql/
│   └── queries.sql
├── dashboard/
│   └── loan_approval.pbix
├── images/
├── README.md
└── requirements.txt
```
> Adjust this to match what you actually upload.

## How to Run
```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook notebooks/loan_approval_analysis.ipynb
```
Or open the notebook directly in Google Colab and upload `loanapproval.csv`.

## Limitations
- The dataset is small (1,000 rows) and has no missing values or duplicates, so it may be simulated rather than real bank data.
- Findings show association, not causation.

## Author
**Sherin Kunjumon**
Junior Data Analyst | Power BI · Excel · MySQL · Python
[LinkedIn](https://www.linkedin.com/in/your-profile) · [GitHub](https://github.com/your-username)
