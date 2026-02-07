# Employee Retention Prediction

A machine learning project that predicts which employees are likely to leave a company and identifies the main reasons behind employee turnover.

## What This Project Does

This project analyzes employee data to understand why people leave their jobs and builds a model to predict who might leave next. The goal is to help companies take action before losing valuable employees.

## The Problem

When employees leave, companies lose money on recruitment, training new hires, and decreased productivity. This project helps answer:
- What makes employees want to leave?
- Can we predict who will leave before they do?
- What can companies do to keep their best people?

## The Data

I worked with data from 14,999 employees that included:
- How satisfied they are with their job
- Their last performance review score
- How many projects they work on
- How many hours they work per month
- How long they've been at the company
- Whether they got promoted recently
- Their department and salary level
- Whether they left the company or not

## What I Did

First, I cleaned the data by removing 3,008 duplicate records and fixing inconsistencies. Then I explored the data to find patterns in who was leaving and why.

I built three different prediction models and compared them:

**Logistic Regression:** 83% accuracy (baseline model)

**Decision Tree:** 96.2% accuracy

**Random Forest:** 96.5% accuracy (best model - this is what I used)

The random forest model correctly identified 91% of employees who actually left, which means it can help companies intervene before people quit.

## What I Found

The analysis revealed three types of employees who leave:

**Overworked High Performers**
These are the best employees working 240+ hours per month with excellent reviews. They're burning out and leaving despite doing great work.

**Four-Year Veterans**
Employees who've been at the company for exactly 4 years show unusually high turnover. Something happens at this point that makes people want to leave.

**Disengaged Workers**
People with very low job satisfaction who are either not challenged enough or underperforming.

The most important factors predicting turnover are:
1. Performance evaluation scores
2. Number of projects assigned
3. How long they've been at the company
4. Whether they're overworked
5. Job satisfaction levels

## Key Recommendations

Based on the analysis, companies should:
- Limit employees to maximum 5 projects at once
- Pay special attention to employees at their 4-year mark
- Fix the promotion problem (only 2.1% got promoted in 5 years)
- Either compensate people for overtime or stop requiring it
- Recognize and reward high performers before they leave

## Tools Used

- Python for all the coding
- Pandas for working with the data
- Scikit-learn for building the prediction models
- Matplotlib and Seaborn for creating visualizations

## Files in This Repository

- `Employee_Retention_Analysis.ipynb` - The complete analysis with all code and visualizations
- `Employee_Retention_Project_Report.docx` - Detailed written report with findings and recommendations
- `README.md` - This file

## How to Run This

1. Clone this repository
2. Install required packages: `pip install pandas numpy matplotlib seaborn scikit-learn`
3. Open the Jupyter notebook and run all cells

## Results Summary

The final model achieves 96.5% accuracy in predicting who will leave. This means companies can identify at-risk employees early and take steps to keep them, potentially reducing turnover from 16.6% to under 12%.
