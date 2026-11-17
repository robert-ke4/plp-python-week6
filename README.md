# Python Week 6 Assignment: Exception Handling

## Project Files
* **`safe_tools.py`**: Implements safe utility functions (`safe_divide`, `safe_number`, and `get_field`) using `try-except` blocks to handle runtime exceptions gracefully.

## Question Answer
**Why can an `if` check not catch "abc" on its own when converting strings to integers?**
An `if` check cannot reliably anticipate every formatting or type irregularity in arbitrary user input strings without duplicating complex parsing logic. Furthermore, passing an incompatible string directly into `int("abc")` triggers a runtime `ValueError` immediately rather than evaluating to a false condition, causing the program to crash unless an exception handler is present to catch the error.