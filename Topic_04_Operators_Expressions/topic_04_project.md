# Topic 4 Project: Personal Finance Calculator

## Overview

Build a **Personal Finance Calculator** that takes a user's monthly income and expense data, performs calculations using all five operator types from this topic, and produces a financial summary report.

---

## Part 1 — Data Collection

Ask the user for:
- Monthly salary (float)
- Monthly rent (float)
- Monthly food budget (float)
- Monthly transport cost (float)
- Number of months they want to project savings for (integer)

## Part 2 — Financial Calculations

Using the inputs:
- Calculate total monthly expenses (sum of rent, food, transport)
- Calculate monthly savings (salary minus total expenses)
- Use `+=` or `-=` at least once when computing a running total
- Calculate projected total savings over the number of months given
- Calculate what percentage of salary goes to expenses (use `/` and `*`)
- Check if expenses exceed 70% of salary — store as a boolean

## Part 3 — Financial Report

Display a formatted report that includes:
- All input values with clear labels
- Total monthly expenses
- Monthly savings amount
- Projected savings over the given months
- Expense percentage of salary (rounded to 2 decimal places)
- A spending alert: if expenses exceed 70% of salary, print "WARNING: High expense ratio!" — otherwise print "Spending is within healthy range."
- A savings projection: if monthly savings are positive, print how many months to save GHS 10,000 (use `//` division) — if savings are zero or negative, print "No savings possible at current expense level."

---

## Instructions

- Save your file as `topic_04_finance.py`
- Use each of these at least once: `/`, `//`, `%`, `**`, a comparison operator, `and` or `or`
- Use at least one `+=` or `-=` operator
- Include meaningful comments

---

## Example Output

```
========================================
       PERSONAL FINANCE REPORT
========================================
Monthly Salary     : GHS 3500.00
Rent               : GHS 800.00
Food               : GHS 600.00
Transport          : GHS 200.00
----------------------------------------
Total Expenses     : GHS 1600.00
Monthly Savings    : GHS 1900.00
Expense Ratio      : 45.71%
----------------------------------------
Spending is within healthy range.
Months to save GHS 10000: 5 months
Projected savings (6 months): GHS 11400.00
========================================
```
