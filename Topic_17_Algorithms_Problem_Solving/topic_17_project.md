# Topic 17 Project: Mini Search & Sort Engine

## Overview

Build a **Mini Search & Sort Engine** for a product inventory system.  
This project requires you to implement searching, sorting, and recursion from scratch — do **not** use Python's built-in `sort()`, `sorted()`, or `index()` functions for the core tasks.

---

## Part 1 — Build the Inventory

**Question:**  
Create a list of **at least 10** product records as Python dictionaries.  
Each record must include: `id` (integer), `name` (string), `category` (string), `price` (float), `stock` (integer).

Use at least **3 different categories** (e.g. Electronics, Clothing, Food).

**Instructions:**
- Define the list manually (no CSV loading for this part)
- Print all products in a formatted table with columns: ID | Name | Category | Price | Stock

---

## Part 2 — Sort by Price (Bubble Sort)

**Question:**  
Implement `bubble_sort_by_price(products)` that sorts the product list in **ascending order by price** using bubble sort.

**Instructions:**
- You must implement bubble sort yourself — do not use `sorted()` or `.sort()`
- Include the **early-exit optimisation** (stop if no swaps occurred in a pass)
- Print the sorted list after sorting
- Add a comment stating the Big O of your function and why

---

## Part 3 — Search by ID (Binary Search)

**Question:**  
Implement `binary_search_by_id(products, target_id)` that searches the product list for a product with the given `id`.

**Instructions:**
- The list must be sorted by `id` before searching — sort it first using your bubble sort
- Implement binary search yourself — do not use Python's `index()` or `in` operator
- Return the matching product dictionary, or `None` if not found
- Test your function by searching for at least 2 valid IDs and 1 ID that does not exist
- Add a comment stating the Big O of binary search and why

---

## Part 4 — Total Inventory Value (Recursion)

**Question:**  
Implement `total_value(products, index)` that computes the **total inventory value** (sum of `price × stock` for all products) using **recursion** — no loops allowed in this function.

**Instructions:**
- Base case: when `index` equals `len(products)`, return `0`
- Recursive case: return `products[index]['price'] * products[index]['stock']` + `total_value(products, index + 1)`
- Call the function as `total_value(products, 0)`
- Print the result formatted to 2 decimal places
- Add a comment stating the Big O of your function

---

## Part 5 — Final Report

**Question:**  
Print a formatted summary report that includes:
1. Products sorted by price (from Part 2)
2. The result of at least two search operations (from Part 3)
3. Total inventory value (from Part 4)

---

## Instructions

- Save your solution as `topic_17_search_sort_engine.py` or in a Jupyter notebook
- Do **not** use `sorted()`, `list.sort()`, or `list.index()` for the core algorithm tasks
- Include a **Big O comment** for each of your three main functions
- Add clear comments explaining each major step
- Each question carries the marks shown — total: **20 marks**

| Part | Marks |
|------|-------|
| Part 1 — Build the Inventory | 3 |
| Part 2 — Bubble Sort by Price | 5 |
| Part 3 — Binary Search by ID | 5 |
| Part 4 — Recursive Total Value | 5 |
| Part 5 — Final Report | 2 |
| **Total** | **20** |

---

## Expected Output (Example)

```
=== Product Inventory ===
ID  | Name            | Category    | Price   | Stock
----|-----------------|-------------|---------|------
101 | USB Cable       | Electronics |   5.99  |  200
102 | T-Shirt         | Clothing    |  15.00  |   80
...

=== Sorted by Price ===
ID  | Name            | Category    | Price   | Stock
101 | USB Cable       | Electronics |   5.99  |  200
...

=== Search Results ===
Search ID 103: {'id': 103, 'name': 'Headphones', ...}
Search ID 999: None (not found)

=== Total Inventory Value ===
Total value: GHS 12,450.00
```
