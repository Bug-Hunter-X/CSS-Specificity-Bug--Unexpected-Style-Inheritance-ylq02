# CSS Specificity Bug: Unexpected Style Inheritance

This repository demonstrates a subtle bug related to CSS specificity.  The goal is to style list items differently depending on whether they are inside a navigation menu. However, due to the way CSS specificity works, the styling is not applied as expected.

The `bug.css` file contains the buggy code, while `bugSolution.css` provides a corrected version.

## Bug Description
The issue stems from the fact that the selector `nav li` is more specific than `li`. Thus, even when a list item is not inside a navigation menu, it will still be styled according to the `nav li` rule because of higher specificity.

## Solution
The solution involves understanding and properly managing CSS specificity.  The updated code ensures only list items within the navigation menu are styled with the intended red color while using the most appropriate approach for the problem.