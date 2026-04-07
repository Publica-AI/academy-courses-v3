# Topic 3 Project: Student Report Card Generator

## Overview

Build a **Student Report Card Generator** that collects a student's academic data, validates the data types, and prints a formatted report card with calculated results.

---

## Part 1 — Data Collection and Type Assignment

Ask the user for the following. Store each value in the correct data type:
- Student full name (string)
- Student ID number (integer)
- Three subject scores: Math, English, Science (each as a float)
- Whether the student attended all classes (yes/no — store the answer as a boolean: True if "yes", False otherwise)

## Part 2 — Calculations

Using the values collected:
- Calculate the average score across the three subjects
- Determine the highest and lowest of the three scores (you may use `max()` and `min()`)
- Calculate the total marks out of 300

## Part 3 — Report Card Display

Print a formatted report card that includes:
- A header using `=` characters
- Title: "STUDENT REPORT CARD"
- All collected student details with labels
- The calculated average, highest score, lowest score, and total
- A remark line: if the average is 70 or above, print "Status: PASS" — otherwise print "Status: FAIL"
- Show the data type of at least two variables using `type()`

---

## Instructions

- Save your file as `topic_03_report_card.py`
- Use correct `snake_case` naming for all variables
- Include at least 4 meaningful comments
- Do not use any data structures (lists, dictionaries) — only the four core types

---

## Example Output

```
==========================================
           STUDENT REPORT CARD
==========================================
Name       : Kofi Mensah
Student ID : 10245
------------------------------------------
Subject Scores:
  Math     : 78.5
  English  : 85.0
  Science  : 72.0
------------------------------------------
Average    : 78.5
Highest    : 85.0
Lowest     : 72.0
Total      : 235.5 / 300
------------------------------------------
Full Attendance: True
Status     : PASS
==========================================
```
