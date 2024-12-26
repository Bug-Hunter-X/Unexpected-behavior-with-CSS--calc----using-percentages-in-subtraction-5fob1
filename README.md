# Unexpected behavior with CSS `calc()` using percentages in subtraction

This repository demonstrates an uncommon error related to using percentages in subtraction within the CSS `calc()` function.  Some browsers may not handle this consistently, leading to unexpected layout issues.

The `bug.css` file contains the erroneous code.  The `bugSolution.css` file provides the corrected version.  The issue stems from subtracting a percentage from a percentage within the `calc()` function.  This is generally not how `calc()` is intended to be used and may lead to inconsistent behavior across browsers.  It's best practice to use absolute units (like px, em, rem) or a unit in the second operand for consistent behavior.