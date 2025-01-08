# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating through arrays.
The code attempts to access an array element that is outside the bounds of the array, resulting in an `ArrayIndexOutOfBoundsException`.
The solution shows how to correct the loop condition to avoid this error.

## Bug

The `bug.java` file contains the erroneous code.  The `for` loop's condition `i <= arr.length` is incorrect.  Array indices are zero-based, so the valid indices range from 0 to `arr.length - 1`.

## Solution

The `bugSolution.java` file provides the corrected code.  The loop condition is changed to `i < arr.length` to correctly iterate through the array elements.