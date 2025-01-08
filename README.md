# MongoDB $inc operator error with string value

This repository demonstrates a common error when using the `$inc` operator in MongoDB. The `$inc` operator is used to increment a numerical field by a specified value.  However, if a string is used as the increment value, the operation will fail silently or produce unexpected results.

## Bug Description
The provided code attempts to increment the `counter` field by the string '1'. This is incorrect; the `$inc` operator expects a numerical value.

## Solution
The solution involves ensuring that the value being incremented is a number.  The corrected code increments the `counter` field by the number 1.