# Smart Digital Expense Tracker with Budget Prediction

BCA I Semester (Session 2026-2027), Course BCA111P

**Submitted by:** Devansh Yadav

**Submission files**

- [Lab Report (PDF)](Lab_Report_Expense_Tracker.pdf): objective, algorithm, source code, sample input/output and conclusion
- [Source Code (expense_tracker.cpp)](expense_tracker.cpp)

A menu-driven C++ program that helps a student record daily expenses, categorize spending, monitor a monthly budget and predict whether the budget will be exceeded.

## Features

1. User Registration
2. Login System (3 attempts)
3. Add Daily Expense
4. View Expense History (sorted by date)
5. Category-wise Expense
6. Monthly Expense Report (also saved to a text file)
7. Budget Setting
8. Budget Warning (at 80% and when over budget)
9. Expense Prediction
10. Search Expense (by date, category or word in note)
11. Delete Expense
12. File Saving

## How to run

```bash
g++ expense_tracker.cpp -o expense_tracker
./expense_tracker
```

## How the prediction works

```
average per day   = spent so far / days passed
predicted total   = average per day * days in the month
```

If the predicted total is more than the budget, the program warns the user and shows the most they can spend per day to stay within budget.

## Concepts used

Variables, loops, arrays, structures, functions, file handling, strings, searching (linear search) and sorting (bubble sort).

## Data files

The program creates these text files in the folder it runs from:

| File | Stores |
|---|---|
| `users.txt` | Usernames and passwords |
| `expenses_<username>.txt` | That user's expenses |
| `budget_<username>.txt` | That user's monthly budget |
| `report_<username>_<month>_<year>.txt` | Saved monthly report |

Passwords are stored as plain text, so this is a lab project and should not be used for real passwords.

## Future enhancements

AI-based spending prediction, mobile app, QR bill scanner and cloud backup.
