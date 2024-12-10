# Uncommon innerHTML Behavior in HTML
This repository demonstrates an uncommon bug related to using `innerHTML` to add multiple paragraphs to a div element in HTML.  The issue shows inconsistent rendering across different browsers.  The bug.html file contains the problematic code and bugSolution.html demonstrates a solution.

## Bug Description
When multiple paragraph elements are concatenated and assigned to a div's `innerHTML`, some browsers may fail to render the additional paragraphs correctly.  This inconsistent behavior seems linked to the way innerHTML processes the string input and potentially the browser's handling of DOM manipulation.

## Solution
The preferred approach avoids directly using innerHTML to append multiple elements.  Instead, create DOM elements using `document.createElement()` and append them to the parent element. This offers more control and reduces rendering inconsistencies. 