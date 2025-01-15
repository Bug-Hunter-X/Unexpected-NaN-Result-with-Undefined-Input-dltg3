# JavaScript Bug: Unexpected NaN Result with Undefined Input

This repository demonstrates a common JavaScript bug involving unexpected NaN results when a function receives 'undefined' as an argument.  The `foo` function attempts to handle `null` values correctly, returning 0. However, when passed `undefined`, it produces NaN due to the addition operation.

## Bug Description

The function doesn't explicitly check for `undefined`, leading to unexpected behavior.  A better solution would include handling `undefined` to avoid NaN results. 

## Bug Solution

The solution addresses this issue by explicitly checking for both `null` and `undefined`, ensuring a consistent and predictable output. 

## How to reproduce

1. Clone the repository.
2. Open `bug.js` to see the buggy code.
3. Open `bugSolution.js` to see the corrected code.
4. Run both JavaScript files and observe the difference in output when calling with `undefined` as an argument. 