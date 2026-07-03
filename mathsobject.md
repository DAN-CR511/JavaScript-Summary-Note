The built-in MATH OBJECT are used to tackle more complex challenges.
It provides variety of methods to make it eaisers to perform advanced calculations and manipilate numbers.


COMMON METHOD OF MATH.OBJECT

1.  THE MATH.RANDOM() this method generates a pseudo-random floating point number between 0(inclusive, can be 0) and 1(exclusive, can never be exactly 1).

It's called Pseudo-random because the numbers aren't truly random.
JavaScript uses a mathematical alorgithm to generate numbers that appears random. They are used for games, random selection and websites.

2.  MATH.MIN() AND MATH.MAX() are used to take a set of numbers and return the minimum and maximum value, respectively.
EXAMPLE;

const smallest = Math.min(13,4,5,1);
console.log(smallest);  // smallest = 1.

const largest = Math.max(15,3,5,70);
console.log(largest);  // largest = 70.

3.  MATH.CEIL() AND MATH.FLOOR() is used to round numbers up or down to the nearest whole integer.

MATH.CEIL is used for rounding numbers up.
EXAMPLE;

console.log(math.ceil(4.3));  //  which is 5.

MATH.FLOOR is used for rounding numbers down.
EXAMPLE;

console.log(math.floor(5.7));  // 5

MATH.ROUND() is the hybrid of MATH.CEIL() and MATH.FLOOR(). Because Math.round() act like the both depending on the decimal.

4.  MATH.TRUNC() it used to removes the decimal part of a number, returning only the integer part, without rounding.

5.  MATH.SQRT() it's used in getting the square root of a number.

6.  MATH.CBRT() it's used in getting the cube root of a number.

7.  MATH.ABS() it's used to return the absolute value of a number, turning negative into positive.
EXAMPLE;

console.log(Math.abs(-5));  // = 5.
console.log(Math.abs(5));  // = 5.

ABSOLUTE VALUE IS SIMPLY IT'S DISTANCE FROM 0 ON THE NUMBER LINE, IGNORING WHETHER IT'S POSITIVE OR NEGATIVE.

8.  MATH.POW() it's used to raises a number to a power(or exponent).

Math.pow(base,exponent);
Base: the number you want to multiply.
exponent: how many time a base is multiplied by itself.

EXAMPLE:

console.log(Math.pow(2, 3)); // it also means 2^3 which is 8.

console.log(Math.pow(8, 2)); // it also means 8^2 which is 64.


