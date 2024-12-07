# MongoDB $inc Operator with String Value
This example demonstrates an uncommon error in MongoDB: using a string instead of a number with the $inc operator in an update operation.

The incorrect usage results in the update failing silently. The expected behavior is to increment the numerical field 'count' by 1. Instead, due to the incorrect data type, the operation does not modify the document.

The solution involves ensuring that the value passed to the $inc operator is a number.
