# CSS Specificity and Inheritance Bug

This repository demonstrates an uncommon bug related to CSS specificity and inheritance.  The issue involves unexpected color rendering in nested elements due to the interaction between inheritance and selector specificity.  The bug.css file contains the erroneous CSS, and bugSolution.css provides the corrected version.

## Bug Description

A parent `div` element has a blue color. A paragraph (`<p>`) element inside the `div` has a red color specified directly.  A more specific selector, `div p`, attempts to set the color to green.  The unexpected behavior is that the rendered color may not be green as intended, because of the unexpected behavior of inheritance with high specificity selectors.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the rendered color of the paragraph text.

## Solution

The `bugSolution.css` file provides a corrected solution that ensures the expected color is rendered. This fix clarifies selector priority and avoids ambiguity by ensuring the higher specificity rules are applied correctly and that inheritance is used as expected.