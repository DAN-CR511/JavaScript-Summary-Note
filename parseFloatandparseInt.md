parseFloat()  and parseInt()  are two essential method in JavaScript for converting strings to numbers.
They're particularly useful when dealing with user input or processing data that comes in string format but needs to be treated as numerical values.


parseFloat();    This method parses a string argument and returns a floating point number. It's designed to extract a number from the begining of a string, even if the string contains non-numeric characters later on.
In parseFloat() if it can't find a valid number at the begining of the string, it returns NaN(Not a Number).

EXAMPLE OF HOW IT WORK:  
console.log(parseFloat("3.14 abc"));   // output = 3.14
console.log(parsseFloat("abc 3.14));  // output = NaN.


parseInt();   This method parses a string argument and return an integer. Like parseFloat() it starts from the beginning of the string, but it stops at the first non-digit character.
It returns only the integer part. If it can't find a valid integer at the start of the string, it returns NaN.

EXAMPLE OF HOW THEY WORK:

console.log(parseInt("3.14"));   // 3.
console.log(parseInt(44px));   //  44.
console.log(parseInt("abac123"));   // NaN.

BOTH METHODS IGNORES THE LEADING WHITESPACE:
console.log(parseFloat("    3.14"));  // 3.14
console.log(parseInt("    43"));   // 43

THEY HANDLE PLUS(+) AND MINUS(-) SIGNS AT THE BEGINNING OF THE STRING.
console.log(parseFloat("+3.14"));   // 3.14
console.log(parseInt("-42"));   // -42.

The parseFloat() and parseInt() are powerful methods, but they have some limitations. For instance, it doesn't all the number formats...


Understanding how parseFloat() and parseInt() works allows you to handle more numeric data effectively in your appilications, especially when dealing with user inputs or external data sources.