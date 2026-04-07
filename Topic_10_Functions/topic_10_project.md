# Topic 10 Project: Student Assessment Calculator

## Overview

Build a **Student Assessment Calculator** that uses functions to collect, process, and report student exam results.

---

## Part 1 — Score Collection and Validation

Ask the user to enter a student's name and three exam scores (out of 100).

Then:
- Define a function `get_valid_score(prompt)` that asks for a score and keeps asking until a number between 0 and 100 is entered
- Define a function `collect_scores(name)` that calls `get_valid_score()` three times and returns a tuple of the three scores
- Display the collected scores back to the user

## Part 2 — Calculation and Classification

- Define a function `calculate_average(scores)` that accepts the tuple and returns the average
- Define a function `classify_grade(average, passing_score=50)` that returns the letter grade (A ≥ 80, B ≥ 70, C ≥ 60, D ≥ 50, else F) and uses a default parameter for the passing threshold
- Define a function `get_highest_lowest(scores)` that returns the highest and lowest scores as a tuple

## Part 3 — Report Display

- Define a function `display_report(name, scores, average, grade, highest, lowest)` that prints a formatted report including all the calculated values
- The report must show: student name, individual scores, average, grade, highest score, and lowest score
- In the main program, call all functions in the correct order to produce the complete report

---

## Instructions

- Save your file as `topic_10_student_calculator.py`
- Every calculation must be inside a function — no bare calculation code in the main program
- Use default parameter values where applicable
- Include meaningful comments
- Use f-strings for formatted output

---

## Example Output

```
Enter student name: Amara Mensah
Enter score 1 (0-100): 78
Enter score 2 (0-100): 85
Enter score 3 (0-100): 91

============================================
        STUDENT ASSESSMENT REPORT
============================================
Student    : Amara Mensah
Scores     : 78, 85, 91
Average    : 84.7
Grade      : A
Highest    : 91
Lowest     : 78
============================================
```
