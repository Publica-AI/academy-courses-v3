# Topic 1 Project: Python Learner Profile Generator

## Overview

Build a **Python Learner Profile Generator** — a command-line program that collects information from a new Python student and displays a personalised, formatted profile card.

---

## Part 1 — Data Collection

Ask the user for the following:
- Full name
- Age
- Country of residence
- Programming experience level (Beginner / Intermediate / Advanced)
- Favourite Python application area (e.g., Data Science, Web Development, Automation)
- One personal goal they want to achieve with Python by the end of this course

## Part 2 — Profile Card Display

After collecting all information, display a **well-formatted profile card** that includes:
- A visible border/header using `=` characters (at least 40 characters wide)
- A title: "PYTHON LEARNER PROFILE"
- All 6 pieces of information, clearly labelled
- A separator line between the data and the footer
- A personalised motivational message at the end that includes the student's name

## Part 3 — Python Applications Summary

After the profile card:
- Print a hardcoded list of at least 5 Python application areas
- Use a loop to print each item with a bullet point
- Highlight the item that matches the user's chosen area (e.g., using uppercase or asterisks)

---

## Instructions

- Save your file as `topic_01_profile.py`
- Your code must run without errors
- Include comments explaining each section
- All 6 inputs must be collected and displayed

---

## Example Output

```
==========================================
        PYTHON LEARNER PROFILE
==========================================
Name       : Amara Johnson
Age        : 22
Country    : Ghana
Level      : Beginner
Focus Area : Data Science
Goal       : Build a salary prediction model
------------------------------------------
Python can be used for:
  - Web Development
  - *** DATA SCIENCE *** (your choice!)
  - Automation
  - Cybersecurity
  - Machine Learning
------------------------------------------
Good luck, Amara! Your Python journey starts NOW.
==========================================
```
