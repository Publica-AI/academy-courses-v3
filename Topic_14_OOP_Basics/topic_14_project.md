# Topic 14 Project: Bank Account Manager

## Overview

Build a **Bank Account Manager** using object-oriented programming to model and manage multiple bank accounts.

---

## Part 1 — Define the BankAccount Class

Define a class called `BankAccount` with:
- Class attribute `total_accounts` to track how many accounts have been created
- Instance attributes: `owner` (string), `account_number` (string), `balance` (float, default 0)
- `__init__` method that sets all attributes and increments `total_accounts`
- `__str__` method that returns: `"Account[ACC001] | Owner: Amara | Balance: GHS 500.00"`

Test the class by creating 3 accounts with different owners and balances. Print all three using `print()`.

## Part 2 — Add Transaction Methods

Add the following methods to your `BankAccount` class:
- `deposit(amount)` — adds the amount to balance; raises `ValueError` if amount ≤ 0
- `withdraw(amount)` — subtracts from balance; raises `ValueError` if amount ≤ 0 or amount > balance
- `get_balance()` — returns the current balance

In the main program, perform at least 5 transactions across your 3 accounts. Wrap every transaction in a try/except block to handle invalid amounts or overdrafts gracefully.

## Part 3 — Account Summary and File Export

- Store all 3 accounts in a list
- Find and display the account with the highest balance
- Display the total balance across all accounts
- Save all account details to `accounts.csv` using the csv module (columns: account_number, owner, balance)

---

## Instructions

- Save your file as `topic_14_bank_account.py`
- All account logic must be inside the class — no bare calculations in the main program
- Use f-strings and format balance values to 2 decimal places
- Include meaningful comments

---

## Example Output

```
=== Accounts Created ===
Account[ACC001] | Owner: Amara | Balance: GHS 1000.00
Account[ACC002] | Owner: Kofi  | Balance: GHS 500.00
Account[ACC003] | Owner: Ama   | Balance: GHS 2500.00
Total accounts: 3

=== Transactions ===
Amara deposited GHS 200. New balance: GHS 1200.00
Kofi withdrew GHS 100. New balance: GHS 400.00
Error: Insufficient funds. (Ama tried to withdraw GHS 3000)

=== Summary ===
Highest balance: Ama — GHS 2500.00
Total across all accounts: GHS 4100.00
Records saved to accounts.csv
```
