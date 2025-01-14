# CSS Specificity Bug

This repository demonstrates a subtle bug related to CSS selector specificity.  The issue arises from the incorrect assumption that the last declaration of a style for an element always takes precedence.  In reality, more specific selectors will always override less specific ones, regardless of their position in the stylesheet.

The `bug.css` file contains the problematic code.  The solution, provided in `solution.css`, highlights a way to correct this using a better understanding of CSS selector specificity.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your browser.  Observe the unexpected color of the div element.
3. Open `solution.html` in your browser.  Observe the expected color of the div element using a corrected CSS.

## How to Fix

Understanding CSS selector specificity is key.  More specific selectors (those using IDs, classes, and element names) take precedence over less specific ones.  Refer to the `solution.css` file for a corrected approach. Ensure your CSS declarations are arranged and written to reflect your expected style hierarchy to prevent this sort of unexpected behavior.