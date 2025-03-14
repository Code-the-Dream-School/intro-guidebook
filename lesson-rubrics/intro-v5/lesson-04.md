# Lesson 04: JS Array Methods

**Learning objective**: Students will be able to apply array methods and iterative techniques to manipulate data, construct and utilize higher-order functions that accept or return other functions, and implement callback functions to process results sequentially; they will also use higher-order array methods such as forEach, map, and filter to efficiently iterate through arrays.

You can mark the student's assignment as complete if they: 

- [ ] Have forked the Replit file and submitted their assignment. 
- [ ] `console.log` inputs properly for each of the 15 questions.
- [ ] Use proper syntax and good JavaScript logic to answer the questions. Example outputs below. (Note that some student work variation is expected!)

## Sample Code

```javascript
//--------------- IMPORTANT!!! ---------------

// Use the keyboard shortcut Alt + Z (for PC) or Option + Z (for Mac) to allow word wrap on this document.  Word wrap breaks the lines so you don't have to keep scrolling left and right to read.

//READ THE INFORMATION IN THE BROWSER WINDOW PANEL ON THE RIGHT BEFORE BEGINNING YOUR ASSIGNMENT!!

//---------- OVERVIEW AND INSTRUCTIONS ----------

//----------------------------------
// LESSON 4 ARRAY METHODS
//----------------------------------

//  This is the coding assigment for the fourth week of the Intro to Programming course from Code the Dream. The concepts touched on in this assignment include:

//  - Using Array Methods
//  - Understanding about iterative methods
//  - Learning about callbacks
//  - Creating Higher Order Functions
//  - Using existing Array Higher Order Functions (e.g. forEach(), map(), filter(), etc.)

// In this assignment you will write your own code. Your instructions are listed as "comments", meaning the instructions are grayed out and start with '//' at the beginning of the line of code. Put your answers immediately below the instructions for each question. As mentioned in the Welcome to week 4 information to the right, you'll need to use console logs for all the questions to check your code output. Using a function in a console.log is very similar to how you were using them with variables last week. To invoke/call the function use the syntax:

//  console.log("Q#: ", functionName(anyInput))

// Please be sure to check the output of your called functions and console logs in the Console tab to the bottom right of this screen. If your Console is not showing, click the Inspect Button in the top right (see the Welcome to week 4 information to the right if you need help finding that)  Check to make sure that the output you get in your Console is the expected output.

// ----- Practice JS array methods: forEach -----
//---------- QUESTION 1 ----------
// Create an variable called 'names' and assign it an array of people's names.  Write a function called 'printNames' that uses the forEach array method to log each name in an array to the console.  Remember, since you're using the console.log in the function, you'll just want to call your function and pass it the array of names when testing your code.

// EXAMPLE CALL:
//    let names = ["Juan Marcos", "Aleksandra Ivanov", "Zhang Wei", "Bernice King"];
//    console.log("Q1 printNames:");
//    printNames(names);

// EXAMPLE OUTPUT:
//   Q1 printNames:
//   Juan Marcos
//   Aleksandra Ivanov
//   Zhang Wei
//   Bernice King

// PUT YOUR CODE HERE
function printNames(arr) {
  arr.forEach((name) => console.log(name));
}

let names = ["Juan Marcos", "Aleksandra Ivanov", "Zhang Wei", "Bernice King"];
console.log("Q1 printNames:");
printNames(names);

//---------- QUESTION 2 ----------
// Create a variable called 'trees' and assign it an array of 3 objects.  Each object should have a 'type' property and a 'height' property.  You can use 'type' to describe the type of tree (ex. Dogwood, Maple, Oak, Elm, etc.) and give them any height.  Now write a function called 'logTreeType' that uses forEach to log the type of each tree object to the console.

// EXAMPLE CALL:
//   const trees = [
//     { type: "oak", height: "30m" },
//     { type: "elm", height: "25m" },
//     { type: "birch", height: "18m" } ]
//   console.log("Q2 logTreeType:");
//   logTreeType(trees);

// EXAMPLE OUTPUT:
//   Q2 logTreeType:
//   oak
//   elm
//   birch

// PUT YOUR CODE HERE

function logTreeType(arr) {
  arr.forEach((tree) => console.log(tree.type));
}

const trees = [
  { type: "oak", height: "30m" },
  { type: "elm", height: "25m" },
  { type: "birch", height: "18m" },
];
console.log("Q2 logTreeType:");
logTreeType(trees);

//---------- QUESTION 3 ----------
// Create a variable called 'myNumbers' and assign it an array of numbers.  Now write a function caled 'totalPoints' that uses forEach to add up all the numbers in that array of numbers.

// EXAMPLE CALL:
//   let myNumbers = [1, 2, 7, 5, 8];
//   console.log (`Q3 totalPoints [${myNumbers}]:`, totalPoints(myNumbers));

// EXAMPLE OUTPUT:
//   Q3 totalPoints [1,2,7,5,8]:  23

// Try a few different input arrays to verify your code is working.

// PUT YOUR CODE HERE

function totalPoints(arr) {
  let sum = 0;
  arr.forEach((num) => (sum += num));
  return sum;
}

let myNumbers = [1, 2, 7, 5, 8];
console.log(`Q3 totalPoints [${myNumbers}]:`, totalPoints(myNumbers));

//---------- QUESTION 4 ----------
// Create a variable called 'myWords' and assign it an array of words.  Then write a function called 'buildSentence' that takes in an array of words and uses forEach to add the strings together. It should also add a space, " ", after each word.

// EXAMPLE CALL:
//    let myWords = ["You","can","if","you","think","you","can","!"];
//    console.log (`Q4 buildSentence [${myWords}]: `, buildSentence(myWords));

// EXAMPLE OUTPUT:
//   Q4 buildSentence [You,can,if,you,think,you,can,!]:  You can if you think you can !

// Note: You should have a space after the ! too
// Try a few different input arrays to verify your code is working.

// PUT YOUR CODE HERE

function buildSentence(arr) {
  let sentence = "";
  arr.forEach((word) => (sentence += word + " "));
  return sentence.trim();
}

let myWords = ["You", "can", "if", "you", "think", "you", "can", "!"];
console.log(`Q4 buildSentence [${myWords}]: `, buildSentence(myWords));

//---------- QUESTION 5 ----------
// Create a variable called 'decimals' and assign it an array of decimal numbers.  Write a function called 'logPercentages' that takes an array of decimal numbers and uses forEach to log each one with the numbers formatted as percentages. That means:
//    Multiply by 100
//    Include the percent symbol (%) at the end of the string

// EXAMPLE CALL:
//   let decimals = [0.75, 0.91, 0.2, 1.34];
//   console.log("Q5 logPercentages:");
//   logPercentages(decimals);

// EXAMPLE OUTPUT:
// Q5 logPercentages:
//   75%
//   91%
//   20%
//   134%

// PUT YOUR CODE HERE
let decimals = [0.75, 0.91, 0.2, 1.34];

function logPercentages(array) {
  array.forEach((decimal) => {
    const percentage = (decimal * 100).toFixed(2) + "%";
    console.log(percentage);
  });
}

console.log("Q5: ", logPercentages(decimals));

// ----- Practice JS Array Methods - map -----
// ---------- QUESTION 6 ----------
// Let's practice using the map array method.  Create a variable called 'startingNums' and assign it an array of numbers.  Then write a function called 'addThreeToAll' that uses map to add 3 to each number in an array of numbers.

// EXAMPLE CALL:
//   let startingNums = [4, 41, 832, 72, 89];
//   console.log (`Q6 addThreeToAll [${startingNums}]: `, addThreeToAll(startingNums));

// EXAMPLE OUTPUT:
//   Q6 addThreeToAll [4,41,832,72,89]:  [ 7, 44, 835, 75, 92 ]

// PUT YOUR CODE HERE
let startingNums = [4, 41, 832, 72, 89];

function addThreeToAll(arr) {
  return arr.map((num) => num + 3);
}

console.log("Q6: ", addThreeToAll(startingNums));

// ---------- QUESTION 7 ----------
// Create a variable called 'baseNums' and assign it an array of numbers.  Write a function called 'squareAll' that takes in an array of numbers, and uses map to return an array containing the squares of each of the numbers.  Remember, you can square a number by multiplying it by itself, or by using the exponent operator like so:
// let number = 4
// number * number // 16
// number ** 2 // 16
// Note that the caret operator ^ does NOT mean exponent in JavaScript

// EXAMPLE CALL:
//   let baseNums = [4, 41, 832, 72, 89];
//   console.log (`Q7 squareAll [${baseNums}]:`, squareAll(baseNums));

// EXAMPLE OUTPUT:
//   Q7 squareAll [4,41,832,72,89]: [ 16, 1681, 692224, 5184, 7921 ]

// PUT YOUR CODE HERE
let baseNums = [4, 41, 832, 72, 89];

function squareAll(arr) {
  return arr.map((num) => num ** 2);
}

console.log("Q7: ", squareAll(baseNums));

// ---------- QUESTION 8 ----------
// Write a function called 'allGreetings' that takes an array of names (strings) by using your 'names' variable from question 1. Return an array of greetings (strings). The greetings should each be "Hello, [name], nice to meet you!".  You might find it helpful to use template strings.

// EXAMPLE CALL: (using the names array from question 1)
//   console.log (`Q8 allGreetings [${names}]:`, allGreetings(names));

// EXAMPLE OUTPUT:
// Q8 allGreetings [Juan Marcos,Aleksandra Ivanov,Zhang Wei,Bernice King]: [
//  'Hello, Juan Marcos, nice to meet you!',
//  'Hello, Aleksandra Ivanov, nice to meet you!',
//  'Hello, Zhang Wei, nice to meet you!',
//  'Hello, Bernice King, nice to meet you!'
// ]

// PUT YOUR CODE HERE
function allGreetings(names) {
  return names.map((name) => `Hello, ${name}, nice to meet you!`);
}

console.log("Q8: ", allGreetings(names));

// ---------- QUESTION 9 ----------
// Create a variable called 'users' and assign it an array of objects.  See example on line 153 below.  Write a function called 'getUsernames' that takes in an array of user objects and uses map to return an array of just the usernames.

// EXAMPLE CALL:
//   let users = [
//   {
//     username: "juan.marcos",
//     isAdmin: false,
//   },
//   {
//     username: "aleksandra.ivanov",
//     isAdmin: false,
//   },
//   {
//     username: "zhang.wei",
//     isAdmin: false,
//   },
//   {
//     username: "bernice.king",
//     isAdmin: true,
//   }
//   ];
//
//  console.log (`Q9 getUsernames:`, getUsernames(users));

// EXAMPLE OUTPUT:
//   Q9 getUsernames: [ 'juan.marcos', 'aleksandra.ivanov', 'zhang.wei', 'bernice.king' ]

// PUT YOUR CODE HERE
let users = [
  {
    username: "juan.marcos",
    isAdmin: false,
  },
  {
    username: "aleksandra.ivanov",
    isAdmin: false,
  },
  {
    username: "zhang.wei",
    isAdmin: false,
  },
  {
    username: "bernice.king",
    isAdmin: true,
  },
];

function getUsernames(arr) {
  return arr.map((user) => user.username);
}

console.log("Q9: ", getUsernames(users));

// ---------- QUESTION 10 ----------
// Write a function called 'pluck' that takes in an array of objects and a string representing a key as parameters, and uses the map method to return an array of the values at that key for each of the objects.  For example, if we used the users array from the last exercise, we could do pluck(users, 'username') to get the same results as the last question.  If any of the objects does not have a value at that key, the array should have undefined in that slot.  Hint: Using the square bracket notation, you can access a property of an object using a variable.

// EXAMPLE CALL: (using the users array from Q9)
//   console.log (`Q10 pluck "isAdmin":`, pluck(users, "isAdmin"));

// EXAMPLE OUTPUT:
//   Q10 pluck "isAdmin": [ false, false, false, true ]

// Try testing with username too!

// PUT YOUR CODE HERE
function pluck(arr, key) {
  return arr.map((obj) => obj[key]);
}

console.log("Q10: ", pluck(users, "username"));

// ----- Practice JS methods - filter -----
// ---------- QUESTION 11 ----------
// Write a function called 'evenNumbers' that takes an array as an argument and uses the filter method.  Return only the even numbers from the array of numbers.  Remember - you can find out if a number is even by using the % operator (modulus operator) like this:
//  number % 2 === 0   (gives a true boolean result, for even numbers)

// EXAMPLE CALL:
//   let numberArray = [4, 41, 832, 72, 89, 120, 431, 505, 70];
//   console.log (`Q11 evenNumbers [${numberArray}]:`, evenNumbers(numberArray));

// EXAMPLE OUTPUT:
//   Q11 evenNumbers [4,41,832,72,89,120,431,505,70]: [ 4, 832, 72, 120, 70 ]
//
// If there are no even numbers in the array you make and use, return an empty array.

// PUT YOUR CODE HERE
function evenNumbers(arr) {
  return arr.filter((num) => num % 2 === 0);
}

let numberArray = [4, 41, 832, 72, 89, 120, 431, 505, 70];
console.log("Q11: ", evenNumbers(numberArray));

// ---------- QUESTION 12 ----------
// Write a function called 'greaterThan100' that takes in an array of numbers and uses the filter method.  Return any items in the array that are greater than 100.

// EXAMPLE CALL:
//   let numArray = [4,41,832,72,89,120,431,505,70];
//   console.log (`Q12 greaterThan100 [${numArray}]:`, greaterThan100(numArray));

// EXAMPLE OUTPUT:
//   Q12 greaterThan100 [4,41,832,72,89,120,431,505,70]: [ 832, 120, 431, 505 ]
//
// If there are no numbers greater than 100, return an empty array.

// PUT YOUR CODE HERE
function greaterThan100(arr) {
  return arr.filter((num) => num > 100);
}

let numArray = [4, 41, 832, 72, 89, 120, 431, 505, 70];

console.log("Q12: ", greaterThan100(numArray));

// ---------- QUESTION 13 ----------
// Write a function called 'nonAdminUsers' that takes in an array of user objects.  The objects should have a username and isAdmin property each like they do in Question 9.  The function should use the filter method to return the users who are not admins.

// EXAMPLE CALL: (using users array from Q9)
//   console.log (`Q13 nonAdminUsers:`, nonAdminUsers(users));

// EXAMPLE OUTPUT:
//   Q13 nonAdminUsers: [
//     { username: 'juan.marcos', isAdmin: false },
//     { username: 'aleksandra.ivanov', isAdmin: false },
//     { username: 'zhang.wei', isAdmin: false }
//   ]

// PUT YOUR CODE HERE
function nonAdminUsers(arr) {
  return arr.filter((user) => !user.isAdmin);
}

console.log("Q13 nonAdminUsers: ", nonAdminUsers(users));

// ---------- QUESTION 14 ----------
// Write a function called 'countAdminUsers' that uses filter and the length method on the result from filter.  The function should return the number of users that have 'isAdmin: true' as part of their object.
// EXAMPLE CALL: (using users array from Q9)
//   console.log (`Q14 countAdminUsers:`, countAdminUsers(users));

// EXAMPLE OUTPUT:
//   Q14 countAdminUsers: 1

// It should only count Bernice King since she is the only admin in that example.

// PUT YOUR CODE HERE
function countAdminUsers(arr) {
  return arr.filter((user) => user.isAdmin).length;
}

console.log("Q14: ", countAdminUsers(users));

// ---------- QUESTION 15 ----------
// Write a function called 'shorterThanX' that takes two arguments: an array of strings and an integer.  Use the filter method to return all the strings in the array whose length is shorter than the integer provided as an argument.  If there's no strings in the array that are shorter than the number, return an empty array.

// EXAMPLE ARRAY:
// let strings = [
//   "Four score and seven years ago",
//   "our forefathers brought forth on this continent a new nation",
//   "conceived in liberty",
//   "and dedicated to the proposition that all men are created equal",
//   "Now we are engaged in a great civil war",
//   "testing whether that nation",
//   "or any so conceived and so dedicated",
//   "can long endure.",
// ];

// EXAMPLE CALL1:
//   console.log (`Q15 shorterThanX 20:`, shorterThanX(strings, 20));
// EXAMPLE OUTPUT1:
//   Q15 shorterThanX 20: [ 'can long endure.' ]

// EXAMPLE CALL2:
//   console.log (`Q15 shorterThanX 30:`, shorterThanX(strings, 30));
// EXAMPLE OUTPUT2:
//   Q15 shorterThanX 30: [
//    'conceived in liberty',
//    'testing whether that nation',
//    'can long endure.'
//  ]

// PUT YOUR CODE HERE
function shorterThanX(arr, length) {
  return arr.filter((str) => str.length < length);
}

let strings = [
  "Four score and seven years ago",
  "our forefathers brought forth on this continent a new nation",
  "conceived in liberty",
  "and dedicated to the proposition that all men are created equal",
  "Now we are engaged in a great civil war",
  "testing whether that nation",
  "or any so conceived and so dedicated",
  "can long endure.",
];

console.log(`Q15 shorterThanX 20:`, shorterThanX(strings, 20));
console.log(`Q15 shorterThanX 30:`, shorterThanX(strings, 30));

// ---------- QUESTION 16 ----------
// Write a function called 'onlyStrings' that takes an array that has different types of elements (numbers, booleans, strings, etc.) and uses the filter method to return an array of only the strings.

// EXAMPLE CALL:
//   let manyTypes = [4, "4", "four score", 80, {age: 80}, ["nations"], {type: "free"}, "states"];
//   console.log (`Q16 onlyStrings [${manyTypes}]:`, onlyStrings(manyTypes));

// EXAMPLE OUTPUT:
//   Q16 onlyStrings [4,4,four score,80,[object Object],nations,[object Object],states]: [ '4', 'four score', 'states' ]

// PUT YOUR CODE HERE
function onlyStrings(arr) {
  return arr.filter((element) => typeof element === "string");
}

let manyTypes = [
  4,
  "4",
  "four score",
  80,
  { age: 80 },
  ["nations"],
  { type: "free" },
  "states",
];

console.log(`Q16 onlyStrings [${manyTypes}]:`, onlyStrings(manyTypes));

// ----- Practice JS methods - find -----
// ---------- QUESTION 17 ----------
// Write a function called 'firstOdd' that takes an array of numbers as an argument.  The function should use the find method to find the first odd number in an array.  Remember - you can find out if a number is odd using the % operator like so:
// number % 2 === 1  (gives a true boolean result, for odd numbers)
// If there are no odd numbers, return undefined.

// EXAMPLE CALL:
//   let array = [4,41,832,72,89,120,431,505,70]
//   console.log (`Q17 firstOdd [${array}]:`, firstOdd(array));

// EXAMPLE OUTPUT:
//   Q17 firstOdd [4,41,832,72,89,120,431,505,70]: 41

// PUT YOUR CODE HERE
function firstOdd(arr) {
  return arr.find((number) => number % 2 === 1);
}

let array = [4, 41, 832, 72, 89, 120, 431, 505, 70];

console.log(`Q17 firstOdd [${array}]:`, firstOdd(array));

// ---------- QUESTION 18 ----------
// Write a function called 'divisibleByTen' that takes an array of numbers as an argument.  The function should use the find method to return the first number that is a multiple of 10.  If there are no numbers divisible by 10, return undefined.

// EXAMPLE CALL:
//   let divArray = [4,41,832,72,89,120,431,505,70]
//   console.log (`Q18 divisibleByTen [${divArray}]:`, divisibleByTen(divArray));

// EXAMPLE OUTPUT:
//   Q18 divisibleByTen [4,41,832,72,89,120,431,505,70]: 120

// PUT YOUR CODE HERE
function divisibleByTen(arr) {
  return arr.find((number) => number % 10 === 0);
}

let divArray = [4, 41, 832, 72, 89, 120, 431, 505, 70];

console.log(`Q18 divisibleByTen [${divArray}]:`, divisibleByTen(divArray));

// ---------- QUESTION 19 ----------
// Write a function called 'divisibleByX' that takes two arguments: an array and an integer.  The function should use the find method to return the first number in the array that's divisible by the integer that was passed as an argument.  If there are no values that are divisible by the second argument, return undefined.

// EXAMPLE ARRAY:
//    let numbers = [4,41,832,72,89,120,431,70];

// EXAMPLE CALL 1:
//    console.log (`Q19 divisibleByX ([${divArray}], 10):`, divisibleByX(numbers, 10));
// EXAMPLE OUTPUT 1: (if using the example array above)
//    Q19 divisibleByX ([4,41,832,72,89,120,431,505,70], 10): 120

// EXAMPLE CALL 2:
//    console.log (`Q190 divisibleByX ([${divArray}]. 3):`, divisibleByX(numbers, 3));
// EXAMPLE OUTPUT 2: (if using the example array above)
//    Q19 divisibleByX ([4,41,832,72,89,120,431,505,70]. 3): 72

// EXAMPLE CALL 3:
//    console.log (`Q19 divisibleByX ([${divArray}], 2):`, divisibleByX(numbers, 2));
// EXAMPLE OUTPUT 3: (if using the example array above)
//    Q19 divisibleByX ([4,41,832,72,89,120,431,505,70], 2): 4

// PUT YOUR CODE HERE
function divisibleByX(arr, num) {
  return arr.find((number) => number % num === 0);
}

let numbers = [4, 41, 832, 72, 89, 120, 431, 70];

console.log(`Q19 divisibleByX ([${divArray}], 10):`, divisibleByX(numbers, 10));
console.log(`Q19 divisibleByX ([${divArray}]. 3):`, divisibleByX(numbers, 3));
console.log(`Q19 divisibleByX ([${divArray}], 2):`, divisibleByX(numbers, 2));

// ---------- QUESTION 20 ----------
// Write a function called 'startsWithLetter' that takes two arguments: an array of strings and a letter.  The function should use the find method to return the first string in the array that starts with the letter provided as the argument.  If there's no string in the array that starts with that letter, return undefined. The function should leave lowercase and uppercase letters alone.
// STRETCH GOAL: Throw an error "Letter must be a string of length 1" if the second argument is not a string, or if its length is more than 1.

// EXAMPLE ARRAY:
// let jokeStrings =
//   ["Do you want to hear a joke?",
//    "It's about a three-legged dog",
//    "The dog walks into a bar",
//    "The dog says, ",
//    "\"I'm looking for the man who shot my paw\"",
//    "Get it?"]

// EXAMPLE CALL 1:
//    console.log (`Q20 startsWithLetter T:`, startsWithLetter(jokeStrings, "T"));
// EXAMPLE OUTPUT 1: (if using the example array above)
//    Q20 startsWithLetter T: The dog walks into a bar

// EXAMPLE CALL 2:
//    console.log (`Q20 startsWithLetter I:`, startsWithLetter(jokeStrings, "I"));
// EXAMPLE OUTPUT 2: (if using the example array above)
//    Q20 startsWithLetter I: It's about a three-legged dog

// EXAMPLE CALL 3:
//    console.log (`Q20 startsWithLetter i:`, startsWithLetter(jokeStrings, "i"));
// EXAMPLE OUTPUT 3: (if using the example array above)
//    Q20 startsWithLetter i: undefined

// STRETCH GOAL EXAMPLE CALL:
//    console.log (`Q20 startsWithLetter dog:`, startsWithLetter(jokeStrings, "dog"));
// STRETCH GOAL EXAMPLE OUTPUT:
//    Q20 startsWithLetter dog: Error: Letter must be a string of length 1

// PUT YOUR CODE HERE
function startsWithLetter(strings, letter) {
  return strings.find((string) => string.charAt(0) === letter);
}

let jokeStrings = [
  "Do you want to hear a joke?",
  "It's about a three-legged dog",
  "The dog walks into a bar",
  "The dog says, ",
  '"I\'m looking for the man who shot my paw"',
  "Get it?",
];

console.log(`Q20 startsWithLetter T:`, startsWithLetter(jokeStrings, "T"));
console.log(`Q20 startsWithLetter I:`, startsWithLetter(jokeStrings, "I"));
console.log(`Q20 startsWithLetter i:`, startsWithLetter(jokeStrings, "i"));
```
