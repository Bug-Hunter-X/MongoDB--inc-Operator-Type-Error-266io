# MongoDB $inc Operator Type Error
This example demonstrates a common error when using the `$inc` operator in MongoDB update operations. The error occurs when attempting to increment a numeric field using a string value instead of a number.  The solution shows the correct way to increment the count field.

## Bug
The bug lies in the incorrect usage of the `$inc` operator.  The `count` field should be incremented by a numeric value, but instead, a string ("10") is provided. This leads to an unexpected result, where the update either fails silently or the `count` field is not incremented correctly.

## Solution
The solution involves providing a numeric value (10) instead of a string ("10") to correctly increment the `count` field using the `$inc` operator.