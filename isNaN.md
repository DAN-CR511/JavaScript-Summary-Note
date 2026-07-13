            HOW DOES isNaN WORK.

NaN stands for "Not a Number". It's a special value that represent an unrepresentable or undefined numerical result.
NaN usually appears when javascript tries to perform arithmetic but cannot produce a valid number.

NaN is a property of a GLOBAL PROJECT. It's also considered a type of number in JavaScript that seems counterintuitive at first.
NaN is also contagious, If any arithmetic involves NaN, the result usually becomes NaN...

NaN is typically the result of operations that should return a number but can't produce a meaningful numeric value...

One peculiar property of NaN is that, IT'S NOT EQUAL TO ANYTHING OR ITSELF.
Example; console.log(NaN === NaN);  // IS EQUAL FALSE.

The isNaN() funtion property is used to determine whether a value is NaN or not.
isNaN first converts it value into a number. Then checks if it's NaN.

Due to potential inconsistencies, The Number.isNaN() introduced The sixth edition of JavaScript released in 2015.
The Number.isNaN method does not attempt to convert the parameter to a number before testing. It only returns TRUE if the value is exactly NaN.

The Number.isNaN() provides a more reliable way to check for NaN values especially in cases where type coercion might lead to unexpected results with the global isNaN() function.

When dealing with numerical operations or user inputs that should be numbers, it's often necessary to check for NaN to handle errors or unexpected inputs gracefully...

Understanding NaN and how to properly check for it is crucial for writing robust JavaScript code, especially when dealing with mathematical operations or parsing user inputs...