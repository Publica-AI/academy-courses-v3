# Topic 16 Project: Sales Data Analyser

## Overview

Build a **Sales Data Analyser** that uses Pandas, NumPy, and Matplotlib to load, analyze, and visualize a sales dataset.

---

## Part 1 — Data Creation and Loading

Create and save a CSV file called `topic_16_sales.csv` with at least 10 rows and the following columns: product, category, units_sold, unit_price, month.

Use at least 3 different products, 2 categories (e.g., Electronics, Clothing), and months 1–6.

Read the CSV into a Pandas DataFrame. Display:
- The first 5 rows using `.head()`
- The DataFrame shape and column information using `.info()`

## Part 2 — Analysis

Add two new columns to the DataFrame:
- `revenue` = units_sold × unit_price
- `revenue_category` = 'High' if revenue ≥ 500 else 'Low'

Then calculate and print:
- Total revenue across all rows
- The product with the highest total revenue (group by product)
- The month with the highest revenue
- The number of 'High' revenue transactions

Save the enriched DataFrame to `topic_16_sales_report.csv`.

## Part 3 — Visualizations

Create three charts:
- A bar chart showing total revenue per product
- A line chart showing total revenue per month (sorted by month number)
- A pie chart showing revenue split by category

Each chart must have a title and labeled axes. Display all three charts.

---

## Instructions

- Save your file as `topic_16_sales_analyser.py` or in a Jupyter notebook
- Use `import numpy as np`, `import pandas as pd`, `import matplotlib.pyplot as plt` at the top
- Use `pd.read_csv()` — do not hardcode the data in the analysis section
- Include comments explaining each analysis step

---

## Example Output

```
=== Sales Data ===
  product    category  units_sold  unit_price  month
  Phone      Electronics    5        200.0       1
  T-shirt    Clothing      10         25.0       1
  ...

Shape: (10, 5)

=== Analysis ===
Total revenue: GHS 4250.00
Top product  : Phone (GHS 1800.00)
Best month   : Month 3 (GHS 950.00)
High revenue transactions: 4

Report saved to topic_16_sales_report.csv
[Charts displayed]
```
