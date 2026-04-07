# Topic 6 Project: Multiplication Table and Number Analyzer

## Overview

Build a **Number Analyzer** that uses all four loop concepts — `while`, `for`, `range()`, `break`, and `continue` — to analyze a number and generate useful outputs.

---

## Part 1 — Multiplication Table (for loop + range)

Ask the user for a number between 1 and 12. Validate the input using a `while` loop — keep asking until a valid number is entered.

Then use a `for` loop with `range()` to print the full multiplication table for that number (1 through 12).

## Part 2 — Divisibility Counter (while loop)

Using a `while` loop, count how many integers from 1 to 100 are divisible by the user's number. Use `continue` to skip numbers that are not divisible, and `break` when you have found 10 divisible numbers (stop counting after the first 10).

Display:
- Each of the first 10 divisible numbers found
- The total count found before stopping

## Part 3 — Even Multiples Finder (for loop + break + continue)

Using a `for` loop over `range(1, 200)`:
- Use `continue` to skip any number that is NOT a multiple of the user's number
- Use `continue` again to skip multiples that are odd
- Collect even multiples only
- Use `break` when you have found 5 even multiples
- Display the 5 even multiples found

---

## Instructions

- Save your file as `topic_06_loops.py`
- Each of these must appear at least once: `while`, `for`, `range()`, `break`, `continue`
- Use the input validation loop before processing
- Include at least 3 meaningful comments

---

## Example Output (for input number = 3)

```
Enter a number (1-12): 3

Multiplication Table for 3:
  3 x  1 =  3
  3 x  2 =  6
  ...
  3 x 12 = 36

First 10 numbers (1-100) divisible by 3:
3 6 9 12 15 18 21 24 27 30
Total found: 10

First 5 EVEN multiples of 3:
6 12 18 24 30
```
