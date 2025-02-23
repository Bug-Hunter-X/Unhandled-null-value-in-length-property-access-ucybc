# JavaScript Bug: Unhandled Null Value in Length Property Access

This repository demonstrates a common JavaScript error: attempting to access the `length` property of a null value.  The `bug.js` file contains the erroneous code, while `bugSolution.js` provides a corrected version.

## Bug Description

The function `foo` attempts to return the length of the input `x`. However, it doesn't explicitly handle the case where `x` is null.  This leads to a `TypeError` when `x` is null, as the `length` property cannot be accessed on a null value.

## Solution

The solution in `bugSolution.js` adds a check for `x` being null before accessing `x.length`.  If `x` is null, it returns 0; otherwise, it proceeds as before. This prevents the error and handles the null case gracefully.

## How to Run

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in your preferred JavaScript environment.
3. Execute both files, observing the difference in behavior when `x` is null.