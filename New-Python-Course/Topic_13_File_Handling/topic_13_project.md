# Topic 13 Project: Student Records Manager

## Overview

Build a **Student Records Manager** that saves and loads student data from a CSV file, giving your program persistent data storage.

---

## Part 1 — Writing Student Records

Ask the user to enter details for 3 students (name, score out of 100, and grade letter). Validate each score — it must be between 0 and 100 — and keep asking until a valid score is entered.

Save all 3 records to a file called `students.csv` with columns: name, score, grade. Use `csv.DictWriter` with a proper header row.

## Part 2 — Reading and Displaying Records

Read `students.csv` using `csv.DictReader` and display all records in a formatted report. The report must show:
- All student records with name, score, and grade
- Total number of students
- Average score (formatted to 1 decimal place)
- The student with the highest score

Wrap the file reading in a try/except block to handle the case where the file does not exist yet.

## Part 3 — Append and Search

Ask the user to enter one additional student record and append it to `students.csv` (do not overwrite existing data).

Then ask the user to enter a name to search. Read through the CSV and display the matching student's full record, or display "Student not found" if the name does not match any record.

---

## Instructions

- Save your file as `topic_13_records_manager.py`
- Use `csv.DictWriter` for writing and `csv.DictReader` for reading
- Always open files with `newline=''` and `encoding='utf-8'`
- Use the `with` statement for all file operations
- Include meaningful comments

---

## Example Output

```
=== Add Student Records ===
Student 1 name: Amara
Score (0-100): 85
Grade: A

Student 2 name: Kofi
Score (0-100): abc
Invalid score. Please enter a number between 0 and 100.
Score (0-100): 72
Grade: B

Student 3 name: Ama
Score (0-100): 91
Grade: A

Records saved to students.csv

=== Student Report ===
Name       Score  Grade
Amara       85     A
Kofi        72     B
Ama         91     A
------------------------------
Total students : 3
Average score  : 82.7
Top student    : Ama (91)

Enter new student name: Yaw
Score (0-100): 65
Grade: D
Record appended.

Search by name: Kofi
Found: Kofi | Score: 72 | Grade: B
```
