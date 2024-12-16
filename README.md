# Race Condition in HTML DOM Manipulation

This repository demonstrates a common yet subtle error in HTML: attempting to manipulate a DOM element using JavaScript before it's fully loaded. This can lead to unexpected behavior, including runtime errors.

## Bug Description
The `bug.html` file contains JavaScript code that attempts to change the style of a div element before the element has finished parsing.  This can result in the script failing to find the element, or even worse, causing a runtime error. 

## Solution
The solution is to use the DOMContentLoaded event listener to ensure the script runs only after the entire HTML document is fully loaded. The `bugSolution.html` demonstrates this solution.