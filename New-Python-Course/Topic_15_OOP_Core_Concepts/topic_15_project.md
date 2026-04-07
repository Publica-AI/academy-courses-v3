# Topic 15 Project: School Management System

## Overview

Build a **School Management System** using inheritance, encapsulation, and polymorphism.

---

## Part 1 — Class Hierarchy

Define the following class hierarchy:

`Person(name, age)` — base class with a `__str__` method and an `introduce()` method that prints a basic greeting.

`Student(Person)` — inherits Person; adds `student_id` and a private `__grades` list (initially empty). Include:
- `add_grade(score)` — validates score is 0–100 (raise ValueError if not), then appends to grades
- `get_average()` — returns the average of all grades or 0 if no grades
- `__str__` override that includes student ID and average

`Teacher(Person)` — inherits Person; adds `subject` and a private `__salary`. Include:
- `get_salary()` — returns the salary
- `set_salary(amount)` — raises ValueError if salary < 0
- `teach()` — prints a teaching message with their subject
- `__str__` override that includes subject

## Part 2 — Polymorphism and isinstance

Create a list containing 3 Student objects and 2 Teacher objects. Write a loop that calls `introduce()` on every person in the list polymorphically.

Use `isinstance()` to:
- Count and print the number of students in the list
- Count and print the number of teachers
- Find and display the student with the highest grade average

## Part 3 — File Export

Save all records to `school_records.csv`:
- For students: type, name, student_id, average_grade
- For teacher: type, name, subject, (leave grade column blank)

Use `csv.DictWriter` and the `with` statement.

---

## Instructions

- Save your file as `topic_15_school_system.py`
- All data and logic must be inside the appropriate classes
- Use `@property` or getter/setter for private attributes
- Use try/except where appropriate for invalid inputs
- Include meaningful comments

---

## Example Output

```
=== All Staff and Students ===
Hi, I am Amara Mensah, age 20. I am a student (ID: STU001).
Hi, I am Kofi Boateng, age 22. I am a student (ID: STU002).
Hi, I am Ama Asante, age 21. I am a student (ID: STU003).
Hi, I am Mr. Nkrumah, age 45. I teach Python Programming.
Hi, I am Ms. Owusu, age 38. I teach Data Science.

Students: 3 | Teachers: 2

Top student: Amara Mensah — Average: 87.3
Records saved to school_records.csv
```
