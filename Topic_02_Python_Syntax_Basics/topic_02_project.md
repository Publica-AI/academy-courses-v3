# Topic 2 Project: Smart User Registration Form

## Overview

Build a **Smart User Registration Form** — an interactive command-line program that collects registration details from a user and displays a formatted confirmation summary.

---

## Part 1 — Data Collection

Ask the user for all of the following:
- Full name
- Email address
- Age
- Country
- Course of interest (Python Basics / Web Development / Data Science / Cybersecurity)
- Preferred study time (Morning / Afternoon / Evening)

Each prompt must be clearly worded so the user knows exactly what to type.

## Part 2 — Time-Based Greeting

Based on the user's preferred study time, display a personalized greeting:
- "Morning" — `"Good morning, [name]! Early birds get the best grades."`
- "Afternoon" — `"Good afternoon, [name]! The afternoon is a great time to focus."`
- "Evening" — `"Good evening, [name]! Night owls are welcome here!"`
- Any other input — `"Welcome, [name]! We'll accommodate your schedule."`

Use a properly indented `if/elif/else` block.

## Part 3 — Registration Summary Card

Display a formatted registration card with:
- A header using `=` characters (at least 42 wide)
- Title: "REGISTRATION CONFIRMED"
- All 6 collected fields with consistent labels
- A separator line between the data and footer
- The user's age displayed as a number (convert using `int()`)
- A footer line: `"Registration ID: PY-[first 3 letters of name in UPPERCASE]-[age]"`

For example, if name is "Amara" and age is 22 the ID would be: `PY-AMA-22`

---

## Instructions

- Save your file as `topic_02_registration.py`
- Your code must run without errors
- Include at least 5 meaningful comments explaining WHY, not just what
- All variable names must be descriptive

---

## Example Output

```
==========================================
         REGISTRATION CONFIRMED
==========================================
Full Name  : Amara Mensah
Email      : amara@example.com
Age        : 22
Country    : Ghana
Course     : Data Science
Study Time : Evening
------------------------------------------
Registration ID: PY-AMA-22
Thank you for registering, Amara Mensah!
==========================================
```
