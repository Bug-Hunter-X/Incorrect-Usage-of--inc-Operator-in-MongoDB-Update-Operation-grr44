# Incorrect Usage of $inc Operator in MongoDB Update Operation
This repository demonstrates an uncommon bug related to the incorrect usage of the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment or decrement a numerical value in a document. However, providing a string value will lead to an error.

## Bug Description
The bug arises from providing a string value to the `$inc` operator instead of a numerical value.  This results in a failure of the update operation.

## Bug Solution
The solution involves ensuring that the value passed to the `$inc` operator is a number (integer or float).