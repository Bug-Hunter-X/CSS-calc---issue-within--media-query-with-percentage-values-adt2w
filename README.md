# CSS calc() Issue within Media Queries

This repository demonstrates a bug related to the unexpected behavior of the `calc()` function in CSS when used with percentage values inside `@media` queries.  The issue is specifically observed when subtracting a fixed pixel value from a percentage value.

## Bug Description

The `calc()` function, when used within a `@media` query to calculate a width based on percentage and pixel subtraction, produces unexpected results. The calculation does not accurately reflect the intended result.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` to see the problematic code.
3. Open `bugSolution.css` for the corrected version.
4. Create an HTML file referencing these CSS files. Observe the differences in behavior.

## Solution

The solution involves correctly using the `vw` unit (viewport width) within the `calc()` function to ensure the calculation is accurate.

## Additional Notes

This issue highlights the importance of understanding how `calc()` interacts with different units within the context of media queries.