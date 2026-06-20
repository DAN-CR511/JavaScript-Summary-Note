Conditional Statement is used for making decisionin javascript.They allow your program to flow in a particular way based on certain conditions.

Ternary Operator lets you control the flow of your code.

IF STATEMENT; it takes a condition and runs a block of code if that condition is TRUTHY.

TRUTHY VALUES are any values that result in a TRUE when evaluted in a boolean context like an IF statement.
examples of TRUTHY VALUE;
Non-empty strings, for example(hello).
Numbers other than 0 and -0, for example(4 & -5).
Arrays.
Objects.
Boolean(true).

FALSY VALUES are values that evaluate to FALSE in a boolean context, which makes them easy to remember..
Example of FALSY VALUES;
Boolean(FALSE).
0(zero).
NaN(not a number).
""(empty string).
null.
undefined.

When using a FALSY VALUE in a code, the message inside the block will never be logged to the console.
But if using TRUTHY VALUE in a code, the message inside the block will be considered TRUE in a boolean context of the IF statement.

Example of how an IF statement work with different Comparison Operators.

Const age = 22;
if (age >= 18) {
    console.log("you are eligible to vote");
}

in this eample, since age is currently 22, it means the condition will evaluate to TRUE because 22 is greater than or equal to 18. so the message "You're eligible to vote" will be logged to the console.


const age = 15;
if (age >= 18) {
    console.log("You're not eligible to vote");
}

In this example age is now 15, then the condition will evaluate to FALSE and the message will not be logged to the console.

WHEN A CONDITION IS FALSE, THEN YOU CAN USE THE ELSE CLAUSE;

const age = 15;
if (age >= 18) {
    console.log("You're eligible to vote");
} else {
    console.log("You're not eligible to vote");
}

ELSE IF BLOCK IS USE FOR MULTIPLE CONDITIONS. It allows your program to choose between more than two paths.

const score = 87;
if (score >= 90) {
    console.log('You got an A');
}
 else if (score >= 80) {
    console.log('You got a B');
 } else if (score >= 70) {
    console.log('You got a C');
 } else {
    console.log('You failed! you need to study more!');
 }

 since the score is currently 87, then the message of You got a B would be logged to the console.

 THE TERNARY OPERATOR  is a compact way to write simple IF/ELSE statements. It has 3 parts; A CONDITION, A RESULT IF THE CONDITION IS TRUE, & A RESULT IF IT'S FALSE.

 Basic Syntax:
 CONDITION ? ExpressionIfTrue : expressionIfFalse;

 example using weather temperature in celsuis:

const temp = 30;
const weather = temp > 25 ? 'sunny' : 'cool';

console.log(`it's a ${weather} day!`);

Here, the temp is greater than 25, the code above logs IT'S A SUNNY DAY!. If temp is ever less than or equal to 25, It logs IT'S A COOL DAY!.

TERNARY OPERATOR is use when dealing with single condition/expressions or when you want a compact syntax for simple logic.

IF/ELSE statement are used when dealing with complex condition and multiple statements.
