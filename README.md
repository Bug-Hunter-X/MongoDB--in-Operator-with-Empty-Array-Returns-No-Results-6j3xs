# MongoDB $in Operator with Empty Array
This example demonstrates a common error when using the `$in` operator with an empty array in MongoDB queries.

The query `db.collection.find({ field: { $in: [] } })` will always return an empty array, regardless of the contents of the collection.

The solution is to avoid using `$in` with empty arrays altogether, or to modify the logic to handle cases where the array is empty.   Consider using other operators or alternative query strategies if an empty array is a possibility.