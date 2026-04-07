# Topic 8 Project: Student Gradebook Manager

## Overview

Build a **Student Gradebook Manager** that uses lists and tuples to store, process, and analyze student grade data.

---

## Part 1 — Gradebook Setup

Create a list of at least 5 student records. Each record must be a **tuple** containing: (student name, exam score, coursework score).

Then:
- Print all records using a `for` loop with `enumerate()` (numbered list)
- Add two new student records using `.append()`
- Remove one student by name using `.remove()` — ask the user which name to remove
- Display the updated list

## Part 2 — Grade Analysis

Iterate over the gradebook list and compute:
- Each student's final score: exam (60%) + coursework (40%)
- The highest final score and which student achieved it
- The lowest final score and which student achieved it
- The class average final score
- How many students scored 70 or above (a Pass mark)

Store final scores in a separate list built using a `for` loop and `.append()`.

## Part 3 — Report Display

Print a formatted gradebook report with:
- A header with student count
- Each student's name and final score (using f-strings)
- Summary statistics: highest, lowest, average, pass count
- A tuple that stores: (subject, highest_score, lowest_score, average) — display it with tuple unpacking

---

## Instructions

- Save your file as `topic_08_gradebook.py`
- All student records must be stored as tuples inside a list
- Use `.append()` to build the final scores list
- Use at least one `.remove()` or `.pop()`
- Use `enumerate()` in at least one loop
- Include meaningful comments

---

## Example Output

```
GRADEBOOK — 7 students

1. Amara Mensah
2. Kofi Asante
...

Updated gradebook (after removing a student):

FINAL GRADE REPORT
==========================================
1. Amara Mensah     : 80.20
2. Kofi Asante      : 75.40
...
------------------------------------------
Highest : Amara Mensah (80.20)
Lowest  : Kweku Boateng (58.30)
Average : 72.15
Passed  : 5 students

Summary tuple: ('Math 101', 80.20, 58.30, 72.15)
```
