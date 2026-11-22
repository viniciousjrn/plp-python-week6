# Week 6 Assignment: Error Handling & Debugging

## Files
- `safe_tools.py`: Contains three error-handled functions (`safe_divide`, `safe_number`, and `get_field`) using `try`/`except` blocks to prevent crashes on bad input.
- `README.md`: Summarizes the assignment, describes the repository files, and explains why a standard `if` check cannot catch `"abc"` before type conversion.

## Question: Why can the `if` check not catch `"abc"` on its own?
A standard `if` check only evaluates values after a conversion succeeds, so calling `int("abc")` directly crashes the program with a `ValueError` before any `if` statement can inspect it. Using a `try`/`except` block catches that `ValueError` during the conversion attempt so the program can return `"Not a number"` safely without crashing.
