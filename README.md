# CSS Calc() Function Unit Inconsistency

This repository demonstrates a common error when using the `calc()` function in CSS: attempting to subtract pixels directly from percentages. This leads to incorrect calculations and potential layout issues.

## The Bug

The `bug.css` file contains CSS code with the incorrect usage of `calc()`. Specifically, pixels are subtracted from percentage values without proper unit conversion, causing the width and height calculations to be invalid.

## The Solution

The `bugSolution.css` file provides the corrected code.  To solve the issue, you need to ensure that all units within the `calc()` function are consistent.  In this case, the solution converts the percentage to pixels based on the parent container's width/height before subtraction.