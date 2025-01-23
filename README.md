# Unexpected Behavior with Modulo Operator in Calculator Function

This repository demonstrates a JavaScript code snippet with a subtle bug. The `calculate` function handles basic arithmetic operations (+, -, *, /), but it lacks handling for the modulo operator ("%)".  This leads to an error if the user attempts to perform a modulo operation.

The `bug.js` file contains the buggy code, while `bugSolution.js` provides a corrected version.

## Bug

The primary issue is the absence of a `case` statement for the modulo operator (%) in the `switch` statement.  When a modulo operation is attempted, the default case (`default: throw new Error('Invalid operator');`) is executed, raising an error.  A more robust solution would explicitly handle the modulo operation.

## Solution

The solution adds a case for the modulo operator to handle this operation correctly.

## How to Run

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in your preferred JavaScript environment (e.g., Node.js, browser console).
3. Execute the functions to observe the behavior of the buggy and corrected versions.