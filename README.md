# JavaScript Function Bug: Handling Undefined Values

This repository demonstrates a common subtle bug in JavaScript related to how functions handle undefined values. The function `foo` intends to return `null` if either input `a` or `b` is null or undefined. However, the current implementation only explicitly checks for null.  This leads to unexpected results when undefined values are passed.  The solution corrects this by checking for both null and undefined values.

## Bug
The `bug.js` file shows the buggy code.  The function should return `null` if either argument is null or undefined. Instead, it returns NaN when undefined values are passed.

## Solution
The `bugSolution.js` file shows the corrected code. The solution modifies the conditional statement to check for both `null` and `undefined` values.