        BINARY LOGICAL OPERATOR.


Binary Logical Operators help you to evaluate two expressions and return a result based on their truthiness.
there 3 most common Binary Logical Operators, which are;
1. Logical AND.
2. Logical OR.
3. Nullish coalescing operator.

 1. Logical AND Operator is represented by (&&):
 it checks if both operand are true and return a result. if both operand are truthy, it returns the secong value...

 EXAMPLE:

 const result = true && "hello";

 console.log(result);  (The text "HELLO" is logged to the console because both operand are TRUE. if either operand is Falsy, it returns a FALSY value).
 while if both operand are FALSY, it returns the first FALSY value.

 The AND Operator is used when you want to check for multiple conditions and ensure that all are TRUE before proceeding.
 EXAMPLE OF THE AND OPERATOR IN MULTIPLE CONDITION:

 if (2 < 3 && 3 < 4) {
    console.log('The IF block runs');
 } else {
    console.log('The ELSE block runs');
 };    ( 2 is less than 3 AND 3 is less than 4, means the sentence "The IF block runs" will be logged to the console).
 

 2. THE LOGICAL OR OPERATOR is represented by (||);
 it checks if at least one operand is TRUHTY. If the first operand is TRUTHY,it returns that value. While if the first operand is FALSY but the second is TRUTHY,the second value will be logged to the console.

    EXAMPLE;
    const result = 0 || 'This is truthy';

    console.log(result); // This is truthy

It's also common to use the Logical OR Operator in IF/ELSE statement like this;

let userInput;

if (userInput || 'Guest') {
    console.log('A user is present');
} else {
    console.log('No user detected');
}   (Since we didn't assign a value to the userInput variable, it is currently UNDEFINED. The conditon in the IF statement checks if either the userInput variable or the string GUEST are truthy. But since the string GUEST is tru in a boolean context like this,the string 'A user is present' will be logged on the console).


3. THE NULLISH COALESCING OPERATOR is represented by (??);
It's more sophisticated than the Logical AND and Logical OR.
it is used in scenarios where you want to return a value only if the fist one is NULL or UNDEFINED.

EXAMPLE OF NULLISH COALESCING OPERATOR;

const result = null ?? 'default';

console.log(result); // default.

THE NULLISH COALESCING OPERATOR is incredibly useful in situations where NULL or UNDEFINED are the only vaules that should trigger a fallback or default value.

EXAMPLE OF A USER'S PREFERENCE SETTINGS;

const 





 
