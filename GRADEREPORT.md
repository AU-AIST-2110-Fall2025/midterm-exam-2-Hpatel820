# Grading Report

**Final Grade: 5.70/10.00**

## Rubric

| Criterion | Points |
|-----------|--------|
| `extract_data` correctly slices, title-cases names, int conversion, extracts grades, and leaves input untouched | **2** |
| `curve_grades` applies the curve (while loop) and caps values at 100 | **1.5** |
| `print_top_performers` prints only qualifying `Name: Score` lines (>= 95) | **1.5** |
| Code quality (required loop choices, clear logic) | **0.7** |


## General Comments

Your solution tells me you need to go back to working through looping patterns. Your comments show that you conceptually know what you wanted to do, but the actual code shows that you are not yet comfortable turning that idea into working syntax.

For example:

by_amount = 0
while by_amount < 0:


This while-condition will never run because 0 < 0 is false.
So the loop body never executes.

This kind of error suggests you are still guessing at how to structure loops, instead of building them step-by-step from predictable patterns.


## Functionality

- tests/test_grader.py::RosterHelperTests::test_curve_grades_values_and_clamping: Failed (0.0 points)
   Error:     AssertionError: <function curve_grades at 0x780175a160c0> != [100, 100, 53]

- tests/test_grader.py::RosterHelperTests::test_extract_data_parses_names_and_grades_title_case: Failed (0.0 points)
   Error:     AssertionError: Lists differ: [] != ['Ana Lopez', 'Priya Singh']

- tests/test_grader.py::RosterHelperTests::test_extract_data_returns_new_lists: Failed (0.0 points)
   Error:     AssertionError: Lists differ: [] != ['Max Jones']

- tests/test_grader.py::RosterHelperTests::test_print_top_performers_prints_name_and_score_for_ge_95: Failed (0.0 points)
   Error:     AssertionError: Lists differ: [] != ['Ben: 95', 'Doug: 100']
