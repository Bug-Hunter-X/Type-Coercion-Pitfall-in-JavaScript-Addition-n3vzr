# Type Coercion Pitfall in JavaScript Addition

This example demonstrates a common JavaScript pitfall involving type coercion during addition.  When adding a number and a string, JavaScript will implicitly convert the number to a string and perform string concatenation instead of numerical addition.

## Bug

The `foo` function is intended to add two numbers. However, when one of the arguments is a string, the result is unexpected string concatenation.

## Solution

The solution involves explicitly converting the inputs to numbers before performing the addition using `parseInt()` or `Number()`. This ensures that the addition operation is performed numerically.