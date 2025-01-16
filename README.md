# JavaScript Hoisting Bug

This repository demonstrates a common JavaScript bug related to variable hoisting.  In JavaScript, variable declarations using `var` are hoisted to the top of their scope, but their assignment remains where it is written in the code. This can lead to unexpected `undefined` values if you try to access a variable before its assignment. 

## Bug Description:
The `bug.js` file contains a function that attempts to log the value of a variable before it's assigned. The result is `undefined` because the variable is hoisted but not initialized.

## Solution:
The `bugSolution.js` file provides a corrected version, ensuring the variable is properly assigned before it's accessed.

## How to Reproduce the Bug
1. Clone the repository.
2. Open `bug.js` in a JavaScript environment.
3. Execute the `myFunc` function and observe the output (undefined).

## How to Fix the Bug
1. Review `bugSolution.js` to understand how the code is corrected.
2. Ensure all variables are properly assigned before they are referenced in your JavaScript code.  Using `let` or `const` instead of `var` can help prevent this issue, as those variables are not hoisted in the same way.