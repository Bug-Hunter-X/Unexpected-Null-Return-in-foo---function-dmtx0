# Unexpected Null Return in foo() function

This repository demonstrates a common yet subtle bug in JavaScript function handling of null values. The `foo()` function is designed to add two numbers; however, its null handling is flawed.

## Bug Description
The `foo()` function returns `null` if either or both of its arguments are `null`. This is problematic because it doesn't consider the possibility of one argument being valid while the other is `null`. A more robust approach would be to return the valid argument if one exists.

## Solution
The improved `foo()` function in `bugSolution.js` handles `null` values more gracefully.  It checks each argument and returns the valid number if one exists; otherwise, it returns `null` only when both arguments are `null`.