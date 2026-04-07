# Topic 12 Project: Personal Utility Toolkit

## Overview

Build a **Personal Utility Toolkit** — a menu-driven program that uses a custom module alongside Python's Standard Library modules.

---

## Part 1 — Custom Module

Create a file called `topic_12_utils.py` containing at least three utility functions:
- `celsius_to_fahrenheit(c)` — converts Celsius to Fahrenheit
- `calculate_bmi(weight_kg, height_m)` — returns the BMI value and category (Underweight < 18.5, Normal 18.5–24.9, Overweight 25–29.9, Obese ≥ 30)
- `generate_password(length=12)` — generates a random password using letters, digits, and at least one special character from the `string` and `random` modules

Each function must include error handling using `raise ValueError` for invalid inputs.

## Part 2 — Main Program

Create `topic_12_main.py` that imports your `topic_12_utils` module plus at least two Standard Library modules (`math`, `random`, `datetime`, or `os`).

Build a loop-based menu with these options:
- 1. Temperature Converter
- 2. BMI Calculator
- 3. Password Generator
- 4. Exit

Each menu option calls the appropriate function from your utils module. All user input must be wrapped in try/except to handle invalid entries gracefully. Use `datetime` to display the current date and time when the program starts.

## Part 3 — Session Summary

When the user selects Exit:
- Display a summary of all actions taken in the session (e.g., "You converted 3 temperatures, calculated 1 BMI, generated 2 passwords")
- Display the total session duration using `datetime`
- Thank the user by name (ask for their name at the start of the program)

---

## Instructions

- Save your files as `topic_12_utils.py` and `topic_12_main.py`
- The utils module must work correctly when imported — do not put menu code inside it
- Use `if __name__ == '__main__':` guard in utils.py
- Include comments explaining each function

---

## Example Output

```
Welcome to your Personal Utility Toolkit!
Enter your name: Amara
Hello Amara! Today is 2026-04-03 | Time: 10:45

=== MENU ===
1. Temperature Converter
2. BMI Calculator
3. Password Generator
4. Exit

Choose: 1
Enter temperature in Celsius: 37
37.0°C = 98.6°F

Choose: 3
Password length (default 12): 
Generated password: aB3#xZm9Lp!q

Choose: 4

=== SESSION SUMMARY ===
Temperatures converted : 1
BMI calculations       : 0
Passwords generated    : 1
Session duration       : 0 min 42 sec
Thank you, Amara! Goodbye.
```
