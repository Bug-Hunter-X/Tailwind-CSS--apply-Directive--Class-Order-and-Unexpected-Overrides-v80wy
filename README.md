# Tailwind CSS @apply Directive: Class Order and Unexpected Overrides

This repository demonstrates a subtle bug related to Tailwind CSS's `@apply` directive.  The issue arises when applying multiple utility classes within the `@apply` directive, where class order seems to affect the final styling outcome. Some classes appear to be unexpectedly overridden, leading to inconsistent styling compared to directly applying these classes.

The `bug.html` file shows the buggy behavior, while `bugSolution.html` presents a solution.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your browser. Observe that the styling isn't as expected.
3. Open `bugSolution.html` and observe the correct styling.

## Solution

The issue is resolved by carefully examining class specificity and potential conflicts within the applied utility classes.  In some cases, refactoring the classes and restructuring the HTML can resolve the conflict or by using more specific classes that would override other classes.