# Topic 11 Project: Safe Number Processor

## Overview

Build a **Safe Number Processor** that robustly handles all user input errors and applies exception handling throughout a multi-function program.

---

## Part 1 — Validated Input

Define a function `get_valid_integer(prompt, min_val, max_val)` that:
- Asks the user for an integer using the given prompt
- Keeps asking (loops) until the user enters a valid integer within the given range
- Catches `ValueError` if the input is not an integer
- Prints a helpful message for invalid input and re-prompts
- Returns the valid integer once entered

Test it by collecting a score (0–100) and an age (1–120) from the user.

## Part 2 — Calculator with Error Handling

Define a function `safe_calculate(a, b, operator)` that:
- Supports the four operators: +, -, *, /
- Raises `ValueError` if the operator is not one of the four valid options
- Handles division by zero without crashing
- Returns the result of the operation

In the main program, wrap the call to `safe_calculate` in a try/except/else/finally block:
- `else` — prints the result formatted to 2 decimal places
- `finally` — prints "Calculation complete."

## Part 3 — Custom Validation with raise

Define a function `validate_age(age)` that:
- Raises `ValueError` if age is below 0
- Raises `ValueError` if age is above 120
- Returns the age if valid

Define a function `validate_temperature(temp)` that:
- Raises `ValueError` if temperature is below -273.15 (absolute zero)
- Returns the temperature if valid

In the main program, collect both values from the user and call both validators inside try/except blocks. Display a summary of valid values.

---

## Instructions

- Save your file as `topic_11_safe_processor.py`
- Every function must include a docstring comment describing what it does
- Do not use bare `except:` — always specify the exception type
- Use f-strings for all output

---

## Example Output

```
Enter a score (0-100): abc
Invalid input. Please enter a whole number.
Enter a score (0-100): 150
150 is out of range (0-100). Try again.
Enter a score (0-100): 85
Score accepted: 85

Enter first number: 10
Enter second number: 0
Enter operator (+, -, *, /): /
Calculation complete.
Error: cannot divide by zero.

Enter age: -5
Validation failed: Age cannot be negative.
Enter age: 25
Age accepted: 25
```
