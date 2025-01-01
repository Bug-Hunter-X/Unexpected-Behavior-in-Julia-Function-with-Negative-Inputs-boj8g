# Julia Function Bug

This repository demonstrates a subtle bug in a Julia function that deals with handling negative numbers.  The function is intended to square the input, regardless of sign, but it produces unexpected results for negative inputs.

The `bug.jl` file contains the buggy code. The `bugSolution.jl` file provides a corrected version.

## Bug Description
The function `my_function` incorrectly handles negative inputs.  It squares them and negates the result, which is not the intended behavior.

## Solution
The solution involves correcting the logic within the `else` block to simply return the square of the absolute value of the input.