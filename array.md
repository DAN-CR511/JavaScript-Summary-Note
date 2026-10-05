An ARRAY is an ordered collection of values, each identified by a numeric index. The values in a JavaScript array can be of different data types; Numbers, Strings, Booleans, Objects and even other arrays.

To create an array in JavaScript, you can use the square brackets[].

EXAMPLE: 

Let fruits = ["apple", "banana", "orange"];

One of the key characteristics of array is that they are zero-indexed, meaning that the first element in array has an index of 0, the second element has an index of 1, 

FOR EXAMPLE:

let fruits = ["apple", "banana", "orange"];
console.log(fruits[0]); // "apple"
console.log(fruits[2]); // "orange"

ARRAY have a special length property that returns the number of elements in the array. You can access this property using the length property.

let fruits = ["apple", "banana", "orange"];
console.log(fruits.length); // 3

Another key characteristics of arrays in JavaScript is that they are dynamic meaning that their size can change after they are created. You can add or remove elements from an array using various array methods, such as Psuh(), Pop(), Shift(),  Unshift(), splice().

ARRAYS ARE USEFUL AND VERSATILE WHEN IT COMES TO DATA STORAGE INSIDE YOUR PROGRAMS.

AN IMPORTANT NOTE: If you try to access an index that doesn't exist in the array, JavaScript will return UNDEFINED.

You can update an element by assigning a new value to a specific index...

FOR EXAMPLE:
let fruits = ["apple", "banana", "cherry"];
fruits[1] = "blueberry";
console.log(fruits); // ["apple", "blueberry", "cherry"]

THIS METHODS ALLOWS YOU TO CHNAGE ANY ELEMENT IN THE ARRAY, AS LONG AS YOU KNOW ITS INDEX

You can also add new elements to an array by assigning a value to an index that doesn't exist.

FOR EXAMPLE:
Let fruits = ["apple", "banana", "cherry"];
fruits[3] = "date";
console.log(fruits); // ["apple", "banana", "cherry", "date"]

Although if you assign a value to an index that is much larger than the current length of the array, you will create undefined elements for the indices in between, which can lead to unexpected behavior...


HOW TO ADD AND REMOVE ELEMENTS FROM THE BEGINNING AND END OF AN ARRAY.

ARRAYS in javascript are dynamic, which means you can eaisly add or remove elements from them...

There are 4 methods for adding and removing elements from the beginning and end of an array: Push(), Pop(), shift(), unshift().

THE PUSH() METHOD; It's used to add one or more element to the end of an array.The return value for the push() method is the new length of the array.

EXAMPLE OF ADDING A NEW FRUIT TO AN EXISTING FURITS ARRAY:

const fruits = ["apple", "banana"];
const newLength = fruits.push("orange");
console.log(newLength); // 3
console.log(fruits); // ["apple", "banana", "orange"]

Why it's possible to add more elements to this fruits array when fruits is a constant... 
It is possible because declaring an array with the const keyword creates a refernce to the array.
An array itself is mutable and can be modified. But you cannot assign a new value to the fruits constant like this:

EXAMPLE:
const fruits = ["apple", "banana"];
fruits = ["This", "will", "not", "work"];
console.log(fruits); // Uncaught TypeError: Assignment to constant variable. 

THE POP() METHOD;  It removes the last element from an array and returns that element...

EXAMPLE:
let fruits = ["apple", "banana", "orange"];
let lastFruit = fruits.pop();
console.log(fruits); // ["apple", "banana"]
console.log(lastFruit); // "orange"

THE UNSHIFT() METHOD; It add one or more element to the beginning of an array and returns its new length. It works similarly with the push() method, but modifies the start of the array instead of the end.

EXAMPLE:
let numbers = [2, 3];
let newLength = numbers.unshift(1);
console.log(numbers); // [1, 2, 3]
console.log(newLength); // 3

THE SHIFT() METHOD; It removes the first element from an array and returns that element. It is also similar to the pop()method, but it works at the beginning of the array instead of the end.

EXAMPLE:
Let colors = ["red", "green", "blue"];
let firstColor = colors.shift();
console.log(colors); // ["green", "blue"]
console.log(firstColor); // "red"

Note that while push() and unshift() can add multiple elements at once, pop() and shift() remove only one element at a time.



THE DIFFERENCE BETWEEN ONE-DIMENSIONAL ARRAY AND TWO-DIMENSIONAL ARRAY.

ARRAY are fundamental data structures used to store collections of elements.

A ONE-DIMENSIONAL ARRAY, often called an array, is like a single row of boxes. Where each item in a one-dimensional array is accessed using a single index.

EXAMPLE OF A ONE-DIMENSIONAL ARRAY:
let fruits = ["apple", "banana", "cherry", "date"];
console.log(fruits[2]); // "cherry"

YOU CAN THINK OF IT AS A SINGLE NAMES OF FRUIT NAMES.

A TWO-DIMENSIONAL ARRAY is essentially an array of arrays. It's used to represent data that has a natural grid-like structure, such as chessboard, a spreadsheet, or pixels in an image..
To access an element in a TWO-DIMENSIONAL ARRAY, you need to indices: one for the row and one for the columns..

EXAMPLE OF A TWO-DIMENSIONAL ARRAY;
let chessboard = [
    ["R", "N", "B", "Q", "K", "B", "N", "R"],
    ["P", "P", "P", "P", "P", "P", "P", "P"],
    [" ", " ", " ", " ", " ", " ", " ", " "],
    [" ", " ", " ", " ", " ", " ", " ", " "],
    [" ", " ", " ", " ", " ", " ", " ", " "],
    [" ", " ", " ", " ", " ", " ", " ", " "],
    ["p", "p", "p", "p", "p", "p", "p", "p"],
    ["r", "n", "b", "q", "k", "b", "n", "r"]
];

console.log(chessboard[0][3]); // "Q"
To access the "Q" in the top row, we use two indices; [0],[3]. The first index, 0 selects the first row, and the second index, 3 selects the fourth columns in that row...

The key difference between ONE-DIMENSIONAL AND TWO-DIMENSIONAL ARRAY lies in how you access and organize the data.
ONE-DIMENSIONAL ARRAY use a single index and are suitable for linear data like list or sequences.
TWO-DIMENSIONAL ARRAY use two indices and are ideal for grid-like data structures..
TWO-DIMENSIONAL ARRAY are actually arrays of arrays. This means each element of the outer array is itself an array.
This nested structure allows for great flexibility but also requires careful handling to avoid errors..

ARRAYS HAVE METHODS LIKE 
.map()
.filter()
.reduce()
.forEach()

ARRAY DESTRUCTURING;

ARRAY DESTRUCTURNG is a feature in JavaScript that allows you to extract values from arrays and assign them to variables in a more concise and readable way..
It's particularly useful when working with arrays and functions that returns multiple values.

EXAMPLE OF ARRAY DESTRUCTURING:
let fruits = ["apple", "banana", "orange"];

let [first, second, third] = fruits;

console.log(first);  // "apple"
console.log(second); // "banana"
console.log(third);  // "orange"

In this example above, we have an array called FURITS with three elements. 
Using array destructuring, we assign the first element to the variable FIRST, the second element to SECOND, and the third element to THIRD. 
This allows us to easily access individual elements of the array without using index notations...

WHAT IT WOULD LOOK LIKE IF WE ACCESSED EACH OF THOSE ELEMENT WITH INDEX NOTATION:
const fruits = ["apple", "banana", "orange"];

const first = fruits[0];
const second = fruits[1];
const third = fruits[2];

console.log(first); // "apple"
console.log(second); // "banana"
console.log(third); // "orange"

ARRAY DESTRUCTURING also allows you to skip elements you're not interested in by using commas.

FOR EXAMPLE:
let colors = ["red", "green", "blue", "yellow"];
let [firstColor, , thirdColor] = colors;

console.log(firstColor); // "red"
console.log(thirdColor); // "blue"

In this example we skipped the second element of the colors array by using an extre comma.

ARRAY DESTRUCTURING is the ability to use default values. If the array has fewer elements than the variables you're trying to assign, you can provide default values.
EXAMPLE:
let numbers = [1, 2];
let [a, b, c = 3] = numbers;

console.log(a); // 1
console.log(b); // 2
console.log(c); // 3
In this example we assign default value 3 to c because the numbers array doesn't have a third element.

THE REST SYNTAX(It's denoted by ...).
It allows you to capture the remaining elements of an array that haven't been destructured into a new array.

EXAMPLE;
let fruits = ["apple", "banana", "orange", "mango", "kiwi"];
let [first, second, ...rest] = fruits;

console.log(first);  // "apple"
console.log(second); // "banana"
console.log(rest);   // ["orange", "mango", "kiwi"]
In this example, first and second capture the first two elements of the fruits array, and rest captures all remaining elements as a new array. 
The rest syntax must be the last element in the destructuring pattern...

ARRAY DESTRUCTURING IS A POWERFUL FEATURE THAT CAN MAKE YOUR CODE MORE CONCISE AND EAISER TO READ. IT'S ESPECIALLY USEFUL WHEN WORKING WITH ARRAYS, AND WHEN YOU NEDD TO EXTRACT SPECIFIC ELEMENTS FROM AN ARRAY...


USING A STRING AND ARRAY METHOD TO REVERSE A STRING.

Reversing a string is a common programming task that can be accomplished in JavaScript using a combination of string and array methods.
The process involes three main steps:
1. SPLITTING THE STRING INTO AN ARRAY OF CHARACTERS. BY USING THE SPLIT() METHOD.
2. REVERSING AN ARRAY. BY USING THE REVERSE()METHOD.
3. JOINING THE CHARACTERS BACK INTO A STRING BY USING THE JOIN()METHOD.

The first step in reversing a string is to convert it into an array of individual characters.

THE SPLIT() METHOD: It divides a string into an array of substrings and specifies where each split should happen based on a given separator. If no separator is provided, the method returns an array containing the original string as a single element.

EXAMPLE OF COMMON SEPARATOR:
An empty string (""), which splits the string into individual characters.

A single space (" "), which splits the string wherever spaces occur.

A dash ("-"), which splits the string at each dash.

EXAMPLE OF USING THE SPLIT() METHOD;
let str = "hello";
let charArray = str.split("");
console.log(charArray); // ["h", "e", "l", "l", "o"]
In this example we used the SPLIT("")empty string separator to convert the string HELLO into an array of its individual charcters...

THE REVERSE() METHOD: It is an array that  reverse the elements of an array in place. This means it modifies the original array rather than creating a new one..

EXAMPLE:
let charArray = ["h", "e", "l", "l", "o"];
charArray.reverse();
console.log(charArray); // ["o", "l", "l", "e", "h"]

THE JOIN() METHOD: It creates and returns a new string by concatenating all the elements in an array, separated by a specified separator string... 
If you want to join the charcters without any separators, you can use the empty string as an argument.

EXAMPLE:
let reversedArray = ["o", "l", "l", "e", "h"];
let reversedString = reversedArray.join("");
console.log(reversedString); // "olleh"

NOTE: STRINGS IN JAVASCRIPT ARE IMMUTABLE, WHICH MEANS YOU CAN'T DIRECTLY REVERSE A STRING BY MODIFYING IT. 
THAT'S WHY WE NEED TO CONVERT IT TO AN ARRAY, REVERSE THE ARRAY, AND THEN CONVERT IT BACK TO  A STRING...