FUNCTIONS are reusable pieces of code that perform a specific task or calculate a value..

EXAMPLE OF DECLARING A FUNCTION:
function greet() {
    console.log("Hello, Jessica!")
}
If we tried to run this code, the message won't appear in the console. Because we need to call the function.

A FUNCTION call, or invocation, is when we actually use or excute the function.
To call a FUNCTION, you will need to reference the function name followed by a set of parenthesis...

EXAMPLE:

function greet() {
  console.log("Hello, Jessica!");
}

greet(); // "Hello, Jessica!"

If we want the message to say "Hello, Nick!" or Hello, Destiny! and we don't want to write a new function each time we greet a different user. 
Instead, we can create a reusable function that uses function parameters and arguments...

PARAMETERS AND ARGUMENTS

PARAMETERS acts as placeholders for the values that will be passed to the FUNCTION when it's called..
ARGUMENTS are the actual values passed to the function when it's called..

EXAMPLE:
function greet(name) {
  console.log("Hello, " + name + "!");
}

greet("Alice"); // Hello, Alice!
greet("Nick"); // Hello, Nick!

The "Name" serves as the PARAMETERS while the strings "Alice" and "Nick" servers as the ARGUMENTS.

When a FUNCTION finishes it's execution, it will always return a value. By default, the return value will be UNDEFINED.
For your FUNCTION to return a specific value, you will need to use the to use the RETURN statement.

EXAMPLE OF USING A RETURN STATEMENT.
function calculateSum(num1, num2) {
  return num1 + num2;
}

console.log(calculateSum(3, 4)); // 7
YOU CAN ALSO USE THE VALUE THAT WAS OUTPUT FROM THE FUNCTION LATER IN YOUR CODE...

ANONYMOUS FUNCTIONS

ANONYMOUS FUNCTION is a function without a name that can be assigned to a variable..

EXAMPLE:
const sum = function (num1, num2) {
  return num1 + num2;
};

console.log(sum(3, 4)); // 7

FUNCTIONS support default parameters, it allows you to set default values for parameters. The default values are used when the function is called without an argument for the parameter

EXAMPLE:
function greetings(name = "Guest") {
  console.log("Hello, " + name + "!");
}

greetings(); // Hello, Guest!
greetings("Anna"); // Hello, Anna!
IT'S DEFAULT VALUE IS "GUEST".

In summary, FUNCTIONS allow you to write reusable and organized code. They can take inputs (parameters), perform actions, and return outputs...
