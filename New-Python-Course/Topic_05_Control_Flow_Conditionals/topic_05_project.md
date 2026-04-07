# Topic 5 Project: Smart Grade Classifier

## Overview

Build a **Smart Grade Classifier** that collects a student's academic scores, calculates a weighted final mark, and produces a full grade report with classification and remarks.

---

## Part 1 — Data Collection and Calculation

Ask the user for:
- Student name
- Exam score out of 100 (float)
- Coursework score out of 100 (float)
- Attendance percentage (float, 0–100)

Calculate the weighted final mark: exam contributes 60%, coursework contributes 40%.

Then apply an attendance bonus: if attendance is 90% or above, add 5 marks to the final score. Cap the final score at 100.

## Part 2 — Grade Classification

Using the final score, determine the grade:
- 80 and above → Grade A
- 70 to 79 → Grade B
- 60 to 69 → Grade C
- 50 to 59 → Grade D
- Below 50 → Grade F

Also determine the pass/fail status:
- Grade A, B, C, or D → PASS
- Grade F → FAIL

Display a different motivational remark for each grade level.

## Part 3 — Report Display

Print a formatted report card showing:
- Student name
- Both input scores and attendance
- The calculated final mark (rounded to 2 decimal places)
- Whether the attendance bonus was applied (Yes/No)
- Final grade and pass/fail status
- A personalized motivational message using the student's name

---

## Instructions

- Save your file as `topic_05_grade_classifier.py`
- Use `if/elif/else` for the grade classification — not a series of separate `if` statements
- Use truthy/falsy at least once (e.g., check if name was entered before processing)
- Include at least 3 meaningful comments

---

## Example Output

```
==========================================
           GRADE REPORT
==========================================
Student    : Amara Mensah
Exam Score : 75.0
Coursework : 88.0
Attendance : 92%
------------------------------------------
Final Mark : 80.20  (Bonus Applied: Yes)
Grade      : A
Status     : PASS
------------------------------------------
Excellent work, Amara! Keep it up!
==========================================
```
