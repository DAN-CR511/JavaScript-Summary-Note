.toFixed() Method is a built in JavaScript function that formats a number usimg fixed- point notation. It's particularly useful when you need to control the number of decimal places in a number , especially for displaying currency values or when working with precise measurements...

The .toFixed() method takes one optional argument, which is the number of digits to appear after the decimal point...  
EXAMPLE OF HOW .toFixed() works:

let num = 3.14567;
console.log(num.toFixed(2));   //  "3.15"
In this example we're limiitng the number of decimal place to 2.

NOTE:  The .toFixed method returns a string not a number. This is because the method is primarily intended for formatting numbers for display, not for further calculations..

.toFixed rounds up when the next digit is 5 or greater, while it rounds down when the next digit is less than 5.. If you call, .toFixed () without arguments, it defailt to 0 decimal places...

The .toFixed can be used particularly when workimg with financial calculations or displaying prices...
EXAMPLE:

let price = 19.99;
let taxRate= 0.08;
let total = price + (price * taxRate);
console.log("Total:$" + total.toFixed(2));   // "21.59"


The .toFixed() method is a powerful tool for formatting numbers in JavaScript, particularly when you need to control the display of decimal places...