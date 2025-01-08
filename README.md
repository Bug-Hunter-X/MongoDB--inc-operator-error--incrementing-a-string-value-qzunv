# MongoDB $inc Operator Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment a numerical value by a specified amount. However, if you attempt to increment a string value, it will not work as expected.

## Bug

The `bug.js` file contains code that attempts to increment a string value using `$inc`. This results in the following error:

```
MongoError: Cannot apply $inc to a value of non-numeric type.
```

## Solution

The `bugSolution.js` file demonstrates the correct usage of the `$inc` operator.  The value to be incremented is a number, and the operation works as expected.

## How to reproduce

1. Make sure you have MongoDB and Node.js installed.
2. Clone this repository
3. Run `bug.js` and observe the error
4. Run `bugSolution.js` and observe the correct result.