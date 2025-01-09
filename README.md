# CSS :nth-child Selector Issue

This repository demonstrates a common issue with the CSS `:nth-child` selector when dealing with lists containing elements other than list items (`<li>`).  The `:nth-child` selector counts all child elements, leading to unexpected styling results if non-list items are present.

The `bug.css` file contains the problematic code, while `bugSolution.css` offers a solution using the `:nth-of-type` selector.

## Problem
The provided CSS attempts to style list items with alternating background colors. However, due to the presence of other elements (e.g., `<br>` tags) within the list, the `:nth-child` selector's counting is skewed, resulting in incorrect styling.

## Solution
The solution involves using the `:nth-of-type` selector, which only counts elements of a specific type (in this case, `<li>`).
