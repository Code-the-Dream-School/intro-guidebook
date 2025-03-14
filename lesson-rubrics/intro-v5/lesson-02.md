# Lesson 02: JavaScript Loops and Arrays

Learning objective: Students will be able to construct efficient solutions to repetitive tasks by designing and implementing loops, particularly 'for' loops, while avoiding common pitfalls such as infinite loops; analyze and manipulate arrays to effectively organize and access data.

## Assignment Rubric

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
// LESSON 2 LOOPS AND ARRAYS
//----------------------------------

//# JavaScript Loops and Arrays
// This is the coding assigment for the second week of the Intro to Programming course from Code the Dream. The concepts touched on in this assignment include:
//   - Simplify Repetitive Tasks with Loops
//   - Working with ‘for’ Loops
//   - Understanding Arrays

// In this assignment you will write your own code. Your instructions are listed as "comments", meaning the instructions are grayed out and start with '//' at the beginning of the line of code. Put your answers immediately below the instructions for each question. As mentioned in the Welcome to week 2 information to the right, you'll need to use console logs for all the questions to check your code output. Using a function in a console.log is very similar to how you were using them with variables last week. To invoke/call the function use the syntax:

//  console.log("Q#: ", functionName(anyInput))

// Please be sure to check the output of your called functions and console logs in the Console tab to the bottom right of this screen. If your Console is not showing, click the Inspect Button in the top right (see the Welcome to week 2 information to the right if you need help finding that)  Check to make sure that the output you get in your Console is the expected output.

// ---------- QUESTION 1 ----------
// Write a function called 'repeat' that takes 1 integer parameter and, using a for or while loop, prints out the string "Hello World!" to the console the same number of times as the parameter. NOTE: for this question, since your console log should be inside your function, you only need to call/invoke the function after you write it rather than call/invoke it inside of a console.log.

// EXAMPLE "LOG":
//    repeat(3);
// EXAMPLE OUTPUT:
//    Hello World!
//    Hello World!
//    Hello World!

// PUT YOUR CODE HERE
function repeat(num) {
  for (let i = 0; i < num; i++) {
    console.log("Hello World! ", i);
  }
}

repeat(5);

// ---------- QUESTION 2 ----------
// Write a function called 'pyramidCounting' that takes 1 integer parameter and returns the sum of all of the numbers between 0 and the parameter.

// EXAMPLE LOG:
//    console.log("Q2: ", pyramidCounting(4));
// EXAMPLE OUTPUT:
//    Q2: 10
// The mathematical explanation of this is 0+1+2+3+4 = 10.

//PUT YOUR CODE HERE
function pyramidCounting(num) {
  let sum = 0;
  for (let i = 0; i <= num; i++) {
    sum += i;
  }
  return sum;
}

console.log("Q2: ", pyramidCounting(5));

// ---------- QUESTION 3 ----------
// Write a function called 'noVowels' that take a string parameter and removes vowels from that string using a loop.

// EXAMPLE LOG:
//    console.log("Q3: ", noVowels(adventurous));
// EXAMPLE OUTPUT:
//    Q3: dvntrs

// PUT YOUR CODE HERE
function noVowels(str) {
  let result = "";
  for (let i = 0; i < str.length; i++) {
    let char = str[i].toLowerCase();
    if (
      char !== "a" &&
      char !== "e" &&
      char !== "i" &&
      char !== "o" &&
      char !== "u"
    ) {
      result += str[i];
    }
  }
  return result;
}

console.log("Q3: ", noVowels("Hello World"));

// ---------- QUESTION 4 ----------
// Write a function called 'vowelCount' that takes 1 string parameter and returns the number of vowels in that string.

// EXAMPLE LOG:
//    console.log("Q4: ", vowelCount('I love to code.'));
// EXAMPLE OUTPUT:
//    Q4: 6

// PUT YOUR CODE HERE
function vowelCount(str) {
  let count = 0;
  for (let i = 0; i < str.length; i++) {
    let char = str[i].toLowerCase();
    if (
      char === "a" ||
      char === "e" ||
      char === "i" ||
      char === "o" ||
      char === "u"
    ) {
      count++;
    }
  }
  return count;
}

console.log("Q4: ", vowelCount("Hello World"));

// ---------- QUESTION 5 ----------
// Write a function called 'numOfOdds' that takes 1 integer parameter and returns the number of odd numbers between 0 and that number, including the number if it's odd. (Hint: Use the modulo operator)

// EXAMPLE LOG:
//    console.log("Q5: ", numOfOdds(15));
// EXAMPLE OUTPUT:
//    Q5: 8

// PUT YOUR CODE HERE
function numOfOdds(num) {
  let count = 0;
  for (let i = 0; i <= num; i++) {
    if (i % 2 !== 0) {
      count++;
    }
  }
  return count;
}

console.log("Q5: ", numOfOdds(10));

// ---------- QUESTION 6 ----------
// Create two variables named 'empty' and 'full'.  Assign an empty array to the 'empty' variable and any array of strings or numbers to the 'full' variable.  Write a function called 'arrayChecker' that returns true if the array passed as a parameter is empty and false if not.  Check both the 'empty' and 'full' variables to make sure they are returning the expected values.

// EXAMPLE LOGS:
//    console.log("Q6 empty: ", arrayChecker(empty));
//    console.log("Q6 not empty: ", arrayChecker(full));
// EXAMPLE OUTPUTS:
//    Q6 empty: true
//    Q6 not empty: false

// PUT YOUR CODE HERE
let empty = [];
let full = [1, 2, 3];

function arrayChecker(arr) {
  if (arr.length === 0) {
    return true;
  } else {
    return false;
  }
}

// Checking the 'empty' variable
console.log("Q6 - empty array: ", arrayChecker(empty));

// Checking the 'full' variable
console.log("Q6 - full array: ", arrayChecker(full));

// ---------- QUESTION 7 ----------
// Write a function called 'getElementAt' that takes an array parameter and an integer parameter.  The function should return the element in the array at the given number index or 'null' if it doesn't exist.  Use your 'full' variable from Question 6 to test.

// EXAMPLE LOGS:
//    console.log("Q7: ", getElementAt(full, 2));
//    console.log("Q7: ", getElementAt(full, 7));
// EXAMPLE OUTPUT: (if the array assigned to variable 'full' is ["dream", 19, "code", 24, 180])
//    Q7: code
//    Q7: null

// PUT YOUR CODE HERE
function getElementAt(arr, index) {
  if (index >= 0 && index < arr.length) {
    return arr[index];
  } else {
    return null;
  }
}

// Using the 'full' variable from Question 6
console.log("Q7: ", getElementAt(full, 2));

// ---------- QUESTION 8 ----------
// Write a function called 'insertInArray' that takes an array parameter, makes a NEW array with the value '0' inserted at the second position in the NEW array.  The function should return the NEW array.  Use your 'full' variable from Question 6 to test.  NOTE: Assigning an array to a new variable does not make a copy, it's another reference to the same array.  To make a copy you can use the slice() method as in this example:
// let newArray = originalArray.slice()
// LEARNING MOMENT: Also console log the variable 'full' to compare the new array to the original.

// EXAMPLE LOG:
//    console.log("Q8: ", insertInArray(full));
//    console.log("original array: ", full);
// EXAMPLE OUTPUT: (if the array assigned to variable 'full' is ["dream", 19, "code", 24, 180])
//    Q8: ["dream", 0, 19, "code", 24, 180]
//    original array: ["dream", 19, "code", 24, 180]

// PUT YOUR CODE HERE
function insertInArray(arr) {
  let newArray = [...arr]; // Create a new array using the spread operator

  newArray.splice(1, 0, 0); // Insert 0 at the second position in the new array

  return newArray; // Return the new array
}

console.log("Q8: ", insertInArray(full));

// ---------- QUESTION 9 ----------
// Write a function called 'compareArrays' that takes two Array parameters (containing numbers or strings only) and returns true if they are equal, false if not.  The purpose of this function should be to look at each element of the two arrays and compare them, returning false when they either hit two items that don't match, or returning false if the two arrays themselves are different lengths. You can test this with the 'empty' and 'full' variables from Question 6, and/or you can create a variable called 'compare' and assign it an array identical to 'full' to compare those.  To further test your function's accuracy, create a new variable called 'part' that is a partial copy of the 'full' variable and test that as well.

// REMEMBER: In JavaScript, 1 === '1' is false, but 1 == '1' is true. You'll need to use the triple equals operator which is more strict because it compares data type.

// EXAMPLE LOG:
//    console.log("Q9 same: ", compareArrays(full, compare));
// EXAMPLE OUTPUT: (if both arrays assigned to variable 'full' and 'compare' are ["dream", 19, "code", 24])
//    Q9 same: true

// EXAMPLE LOG:
//    console.log("Q9 different: ", compareArrays(full, empty));
// EXAMPLE OUTPUT: (if using variables from Question 6)
//    Q9 different: false

// EXAMPLE LOG:
//    console.log("Q9 partial: ", compareArrays(full, part));
// EXAMPLE OUTPUT: (if 'full' variable is ["dream", 19, "code", 24] and if 'part' variable is ["dream", 19, "code"])
//    Q9 different: false

// PUT YOUR CODE HERE
function compareArrays(arr1, arr2) {
  if (arr1.length !== arr2.length) {
    return false;
  }

  for (let i = 0; i < arr1.length; i++) {
    if (arr1[i] !== arr2[i]) {
      return false;
    }
  }

  return true;
}

// Testing with 'empty' and 'full' variables from Question 6
console.log("Q9 - empty and full: ", compareArrays(empty, full));

// Creating a variable 'compare' as a copy of 'full' array
let compare = [...full];
console.log("Q9 - full and compare: ", compareArrays(full, compare));

// Creating a variable 'part' as a partial copy of 'full' array
let part = full.slice(0, 2);
console.log("Q9 - full and part: ", compareArrays(full, part));

// ---------- QUESTION 10 ----------
// Create a variable called 'numbers' and assign it an array with at least 3 numbers as elements (example: [10, 3, 4]).  Write a function called 'calculateTotal' that takes one array parameter and loops through the array in order to return the sum of all the array elements.

// STRETCH GOAL: write another version of calculateTotal (call it calculateTotal2) using the 'reduce()' method

// EXAMPLE LOG:
//    console.log("Q10: ", calculateTotal(numbers));
// EXAMPLE OUTPUT: (if the array assigned to variable 'numbers' is [3, 4, 2 ,8])
//    Q10: 17

// PUT YOUR CODE HERE
let numbers = [10, 3, 4]; // Create a variable called 'numbers' and assign it an array with at least 3 numbers

function calculateTotal(arr) {
  let total = 0; // Initialize a variable 'total' to store the sum

  for (let i = 0; i < arr.length; i++) {
    total += arr[i]; // Add each element of the array to 'total'
  }

  return total; // Return the sum of all array elements
}

// Testing with the 'numbers' array
console.log("Q10 - Total: ", calculateTotal(numbers));

function stretchCalculateTotal(arr) {
  return arr.reduce((accumulator, currentValue) => accumulator + currentValue);
}

// Testing with the 'numbers' array
console.log("Q10 - Stretch Total: ", stretchCalculateTotal(numbers));

// ---------- QUESTION 11 ----------
// Write two functions called 'findEvens' and 'findOdds' that each take one array parameter and each returns a NEW Array of all the even or odd numbers as indicated.  NOTE: Assigning an array to a new variable does not make a copy, it's another reference to the same array.  To make a copy you can use the slice() method as in this example:
// let newArray = originalArray.slice()
// STRETCH GOAL: write another version of findEvens or findOdds using the `filter()` method

// EXAMPLE LOG:
//    console.log("Q11 evens: ", findEvens([10,2,3,19,7,6,93]));
//    console.log("Q11 odds: ", findOdds([10,2,3,19,7,6,93]));
// EXAMPLE OUTPUT:
//    Q11 evens: [10,2,6]
//    Q11 odds: [3,19,7,93]

// PUT YOUR CODE HERE
function findEvens(arr) {
  let evenArray = [];

  for (let i = 0; i < arr.length; i++) {
    if (arr[i] % 2 === 0) {
      evenArray.push(arr[i]);
    }
  }
  return evenArray;
}

function findOdds(arr) {
  let oddArray = [];

  for (let i = 0; i < arr.length; i++) {
    if (arr[i] % 2 === 1) {
      oddArray.push(arr[i]);
    }
  }
  return oddArray;
}

// Testing with any input
console.log("Q11 - findEvens: ", findEvens([1, 2, 3, 4, 5, 6]));
console.log("Q11 - findOdds: ", findOdds([1, 2, 3, 4, 5, 6]));

function stretchFindEvens(arr) {
  let evenArray = arr.filter((num) => num % 2 === 0); // Use the filter method to create a new array of even numbers
  return evenArray;
}

function stretchFindOdds(arr) {
  let oddArray = arr.filter((num) => num % 2 !== 0); // Use the filter method to create a new array of even numbers
  return oddArray;
}

// Testing with any input
console.log("Q11 - Stretch findEvens: ", stretchFindEvens([1, 2, 3, 4, 5, 6]));
console.log("Q11 - Stretch findOdds: ", stretchFindOdds([1, 2, 3, 4, 5, 6]));

// ---------- QUESTION 12 ----------
// Write a function called 'makeSquares' that takes one array parameter and returns a NEW Array with the squared values of each of the numbers.  NOTE: Assigning an array to a new variable does not make a copy, it's another reference to the same array.  To make a copy you can use the slice() method as in this example:
// let newArray = originalArray.slice()
// STRETCH GOAL: write another version makeSquares using the `map()` method

// EXAMPLE LOG:
//    console.log("Q12: ", makeSquares([2,5,8]));
// EXAMPLE OUTPUT:
//    Q12: [4,25,64]

// PUT YOUR CODE HERE
function makeSquares(arr) {
  let squaresArray = [];

  for (let i = 0; i < arr.length; i++) {
    squaresArray.push(arr[i] * arr[i]);
  }

  return squaresArray;
}

// Testing with any input
console.log("Q12 - Squares: ", makeSquares([1, 2, 3, 4, 5]));

function stretchMakeSquares(arr) {
  let squaresArray = arr.map((num) => num ** 2); // Use the map method to create a new array with squared values
  return squaresArray;
}

// Testing with any input
console.log("Q12 - Stretch Squares: ", stretchMakeSquares([1, 2, 3, 4, 5]));

// ---------- QUESTION 13 ----------
// Back in the old days, the early 2000s, this was a famous technical interview question. Write a function definition that takes NO parameters. The function will loop from 1 to 15 and return an array of numbers. While looping, the function will check if the current value in the loop is divisible by 3, by 5, or by both. If the current value in the loop is divisible by 3, the function will add the string "fizz" to an array. If the current value in the loop is divisible by 5, the function will add the string "buzz" to the array. If the current value in the loop is divisible by both, the function will add the value "fizzbuzz" to the array. If the number isn't divisible by 3, 5, OR both, it will add the number to the array.  The function will return the array of values.

// EXAMPLE LOG:
//    console.log("BONUS: ", fizzBuzz();
// EXAMPLE OUTPUT:
//    Q13: [1,2,'fizz',4,'buzz','fizz',7,8,'fizz','buzz',11,'fizz',13,14,'fizzbuzz']

// PUT YOUR CODE HERE
function fizzBuzz() {
  let fizzBuzzArray = [];

  for (let i = 1; i <= 15; ++i) {
    // Check if i is divisible by both 3 and 5
    if (i % 15 === 0) {
      // Add "FizzBuzz" to the result array
      fizzBuzzArray.push("FizzBuzz");
    }

    // Check if i is divisible by 3
    else if (i % 3 === 0) {
      // Add "Fizz" to the result array
      fizzBuzzArray.push("Fizz");
    }

    // Check if i is divisible by 5
    else if (i % 5 === 0) {
      // Add "Buzz" to the result array
      fizzBuzzArray.push("Buzz");
    } else {
      // Add the current number as a string to the
      // result array
      fizzBuzzArray.push(i.toString());
    }
  }
  return fizzBuzzArray;
}

console.log("Q12 - FizzBuzz: ", fizzBuzz());

```
