# CSS Media Query Calc() Error

This repository demonstrates a subtle bug in CSS involving the use of `calc()` within a `@media` query condition.  The provided `bug.css` file contains the erroneous code, while `bugSolution.css` offers the corrected version.  The issue arises from browser inconsistencies in handling calculations directly within media query expressions.

## Bug Description

The `calc()` function is not directly supported within the conditional expression of a `@media` rule in many browsers. Attempting to use it will cause unexpected behavior.  The solution involves performing the calculation before the `@media` condition, creating a variable or using CSS Custom Properties to achieve the desired result.