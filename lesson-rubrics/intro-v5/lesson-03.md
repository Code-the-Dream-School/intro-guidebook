# Lesson 03: JS Objects

**Learning Objective**: Students will be able to differentiate between primitive and object data types, construct and manipulate objects to amend their properties, and apply object destructuring to efficiently access and work with individual values.|

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

//-------------------------------------------
// LESSON 3 OBJECTS
//-------------------------------------------

//# JavaScript Objects
// This is the coding assigment for the third week of the Intro to Programming course from Code the Dream. The concepts touched on in this assignment include:
//   - Object Basics
//   - Primitive vs Object Types
//   - Object Destructuring
//   - Manipulating Objects

// In this assignment you will write your own code. Your instructions are listed as "comments", meaning the instructions are grayed out and start with '//' at the beginning of the line of code. Put your answers immediately below the instructions for each question. As mentioned in the Welcome to week 3 information to the right, you'll need to use console logs for all the questions to check your code output. Using a function in a console.log is very similar to how you were using them with variables last week. To invoke/call the function use the syntax:

//  console.log("Q#: ", functionName(anyInput))

// Please be sure to check the output of your called functions and console logs in the Console tab to the bottom right of this screen. If your Console is not showing, click the Inspect Button in the top right (see the Welcome to week 3 information to the right if you need help finding that)  Check to make sure that the output you get in your Console is the expected output.

// ---------- QUESTION 1 ----------
// Objects are a way to store property:value pairs of data in a variable.  First, create an object called 'myPet'.  Add three properties called 'name', 'species', and 'color' to the 'myPet' object below and assign each of them values.  Use your console.log's to print the values of each property to the console.

// EXAMPLE LOG:
//    console.log("Q1 name: ", myPet.name);
//    console.log("Q1 species: ", myPet.species);
//    console.log("Q1 color: ", myPet.color);
// EXAMPLE OUTPUT:
//    Q1 name: Teddy
//    Q1 species: ferret
//    Q1 color: brown

// PUT YOUR CODE HERE
const myPet = {
  name: "Max",
  species: "Dog",
  color: "Brown",
};

console.log("Q1 name: ", myPet.name);
console.log("Q1 species: ", myPet.species);
console.log("Q1 color: ", myPet.color);

// ---------- QUESTION 2 ----------
// Now let's see how we can use the property:value pairs in template literals.  Create a variable called 'aboutPet' and assign it a template literal that uses the 'myPet' object to make a sentence sharing all the pet details.  The sentence should look something like this: "Teddy is a brown ferret."

// EXAMPLE LOG:
//    console.log("Q2: ", aboutPet);
// EXAMPLE OUTPUT:
//    Q2: Teddy is a brown ferret.

// PUT YOUR CODE HERE
const aboutPet = `${myPet.name} is a ${myPet.color} ${myPet.species}.`;

console.log("Q2: ", aboutPet);

// ---------- QUESTION 3 ----------
// Let's add a method to our object.  Create a method called 'age' that takes no parameters, and uses no outside variables (hint: use 'this').  The method should return the age of the pet in years.

// EXAMPLE LOG:
//    console.log("Q3: ", myPet.age());
// EXAMPLE OUTPUT:
//    Q3: 7

// PUT YOUR CODE HERE

// Don't forget your console.logs!
myPet.petAge = 3;
myPet.age = function () {
  return this.petAge;
};

console.log("Q3: age ", myPet.age());

// ---------- QUESTION 4 ----------
// Now, let's see how we can use data within objects in functions.  Write a function called 'isDog' that takes one object parameter.  In the function, create a variable called 'speciesChecker' and assign it the value 'dog'.  Then, still in the function, return true if the object's species value is equal to the variable 'speciesChecker', or false if not.

// EXAMPLE LOG:
//    console.log("Q4: ", isDog(myPet));
// EXAMPLE OUTPUT: (if your 'myPet' object from Question 1 is about any animal other than a dog)
//    false
// NOTE: if when you made 'myPet' in Question 1, you did put dog as species, you should get true as your output instead.

// PUT YOUR CODE HERE
function isDog(obj) {
  const speciesChecker = "dog";
  return obj.species === speciesChecker;
}

console.log("Q4: ", isDog(myPet));

// ---------- QUESTION 5 ----------
// Now lets work with date and time
// Create a function called 'month'.  Inside the function, declare a variable named 'today' that uses the Date object.  Your function should then return only the month of the 'today' variable.  You can return the month as a number
// STRETCH GOAL: Return the month as a string

// EXAMPLE LOG:
//    console.log("Q5: ", month());
// EXAMPLE OUTPUT: (Will be different for each class but should be the current month.  For example if you're doing this assignment in January...)
//    Q5: 01
//    stretch goal should result in:
//    Q5: January

// PUT YOUR CODE HERE
function month() {
  const today = new Date();
  return today.getMonth() + 1; // Months are zero-based, so add 1
}

console.log("Q5 - Current month: ", month());

function stretchMonth() {
  const today = new Date();
  const monthNames = [
    "January",
    "February",
    "March",
    "April",
    "May",
    "June",
    "July",
    "August",
    "September",
    "October",
    "November",
    "December",
  ];
  return monthNames[today.getMonth()];
}

console.log("Q5 - Stretch - Current month: ", stretchMonth());

// ---------- QUESTION 6 ----------
// Let's explore dates now.  Create a variable named 'birthday' and assign it the date of your next birthday.  Then create a function called 'birthdayCountdown' that takes birthday as a parameter and returns the number of days until your next birthday.  Remember that you may need to use a particular format for your birthday so you can properly convert the data to something you can use in the function.  CAUTION: 2024 is a leap year!

// STRETCH GOAL: As we mentioned in Question 8, you should consider boundary cases. What if the date wasn't formatted to work with your function?

// EXAMPLE LOG:
//    console.log("Q6: ", birthdayCountdown(birthday));
// EXAMPLE OUTPUT: (if your next birthday was March 15, 2024 and today was February 3, 2024)
//    Q6: 41

// PUT YOUR CODE HERE
function birthdayCountdown(birthday) {
  const today = new Date();
  const nextBirthday = new Date(
    today.getFullYear(),
    birthday.getMonth(),
    birthday.getDate()
  );

  // If birthday has already passed this year, set it for next year
  if (nextBirthday < today) {
    nextBirthday.setFullYear(today.getFullYear() + 1);
  }

  // Calculate the difference in milliseconds and convert to days
  const diffTime = nextBirthday - today;
  const diffDays = Math.ceil(diffTime / (1000 * 60 * 60 * 24));

  return diffDays;
}

const birthday = new Date("2025-06-15"); // Change this to your actual next birthday
console.log("Q6: Days until birthday ", birthdayCountdown(birthday));

// ---------- QUESTION 7 ----------
// If we work with dates, we should work with time also.  Create a variable named 'startTime' and assign it a start time.  Create a variable named 'endTime' and assign it an end time.  Then create a function called 'timeDifference' that takes startTime and endTime as parameters and returns the number of hours and minutes between the start and end times.  Remember that you may need to be careful what format you use when entering times so you can properly convert the data to something you can use in the function.

// STRETCH GOAL: You should consider boundary cases. What if the times are not formatted to work with your function?

// EXAMPLE LOG:
//    console.log("Q7: ", timeDifference(startTime, endTime));
// EXAMPLE OUTPUT: (if startTime was 12:37pm and endTime was 3:19pm)
//    Q7: 2 hours and 42 minutes

// PUT YOUR CODE HERE
// Function to calculate the time difference
function timeDifference(startTime, endTime) {
  // Convert startTime and endTime to Date objects
  let start = new Date("1970-01-01T" + startTime + ":00Z");
  let end = new Date("1970-01-01T" + endTime + ":00Z");

  // Calculate the difference in milliseconds
  let difference = end - start;

  // Convert milliseconds to total minutes
  let totalMinutes = difference / 60000;

  // Calculate hours and minutes
  let hours = Math.floor(totalMinutes / 60);
  let minutes = totalMinutes % 60;

  return { hours, minutes };
}

const startTime = "08:30"; // Example start time in HH:MM format
const endTime = "14:45"; // Example end time in HH:MM format
console.log("Q7: ", timeDifference(startTime, endTime));

// ---------- QUESTION 8 ----------
// Create a function called 'absDiff' that takes 2 parameters and returns the absolute difference between them. For example, if the first parameter is smaller than the second, the first parameter will be subtracted from the second. If the first parameter is larger than the second, the second parameter will be subtracted from the first. If they are both equal, return the first parameter subtracted by the second.  It's important to consider boundary cases - situations that may change how you expect your code to behave.  For this reason, work with same numbers and negative numbers as well to see if you get your absDiff function to calculate the absolute difference regardless of number type.

// EXAMPLE LOG 1:
//    console.log("Q8 first larger: ", absDiff(29, 5));
// EXAMPLE OUTPUT: (if using the numbers 29 and 5 as in the example log)
//    Q8 first larger: 24
// EXAMPLE LOG 2:
//    console.log("Q8 second larger: ", absDiff(3, 16));
// EXAMPLE OUTPUT: (if using the numbers 3 and 16 as in the example log)
//    Q8 second larger: 13
// EXAMPLE LOG 3:
//    console.log("Q8 same nums: ", absDiff(5, 5));
// EXAMPLE OUTPUT 3: (if using the numbers 5 and 5 as in the example log)
//    Q8 same nums: 0
// EXAMPLE LOG 4:
//    console.log("Q8 neg num: ", absDiff(-6, 5));
// EXAMPLE OUTPUT 4: (if using the numbers -6 and 5 as in the example log)
//    Q8 neg num: 11

// PUT YOUR CODE HERE
function absDiff(num1, num2) {
  return Math.abs(num1 - num2);
}

// Test cases
console.log("Q8 first larger: ", absDiff(29, 5));
console.log("Q8 second larger: ", absDiff(3, 16));
console.log("Q8 same nums: ", absDiff(5, 5));
console.log("Q8 neg num: ", absDiff(-6, 5));

// ---------- QUESTION 9 ----------
// Create a function called 'convertTemp' that takes 1 temperatue parameter in celsius and return the temperature in Fahrenheit.  Log both the input and output values

// EXAMPLE LOG:
//    console.log("Q9 convertTemp: ", celsiusTemp, convertTemp(celsiusTemp));
// EXAMPLE OUTPUT:
//    Q9 convertTemp: 0 32
// Create logs for several different celsium temperatures

// PUT YOUR CODE HERE
function convertTemp(celsius) {
  let fahrenheit = (celsius * 9) / 5 + 32;
  return fahrenheit;
}

// Test cases
console.log("Q9 convertTemp: ", 0, convertTemp(0));
console.log("Q9 convertTemp: ", 10, convertTemp(10));

// ---------- QUESTION 10 ----------
// Create a function called 'reverseString' that takes 1 string parameter and returns the reverseString.  Log both the input and output values

// EXAMPLE LOG:
//    console.log("Q10 reverseString: ", inputString, reverseString(inputString));
// EXAMPLE OUTPUT:
//    Q10 reverseString: HelloWorld dlroWolleH

// PUT YOUR CODE HERE
function reverseString(input) {
  const reversed = input.split("").reverse().join("");
  return reversed;
}

console.log("Q10 reverseString: ", "Hello", reverseString("Hello"));
console.log("Q10 reverseString: ", "Hello", reverseString("Hello World"));

// ---------- QUESTION 11 ----------
// Declare a variable named "diameter" and assign it an integer value. Through a series of math calculations and variables, calculate the "radius" (which is half the diameter), the "circumference" (which is 2 multiplied by the Math value pi, multiplied by the radius) and the "area" (which is the Math value pi, multiplied by the radius squared).

// PUT YOUR CODE HERE

// Don't forget your console.logs!
let diameter = 10;

// Calculate the radius (half of the diameter)
let radius = diameter / 2;

// Calculate the circumference (2 * pi * radius)
let circumference = 2 * Math.PI * radius;

// Calculate the area (pi * radius^2)
let area = Math.PI * Math.pow(radius, 2);

// Log the results
console.log("Q11 Diameter: " + diameter);
console.log("Q11 Radius: " + radius);
console.log("Q11 Circumference: " + circumference);
console.log("Q11 Area: " + area);

// ---------- QUESTION 12 ----------
// Let's make a useful math problem - create a tip calculator! Declare two variables called "billTotal" and "tipPercentage". Assign billTotal a floating point number with two decimal places. Assign tipPercentage a floating point number between 0.1 and 0.9. Create a third variable called "tip" that will multiply tipPercentage and billTotal then use the addition assignment operator to add that amount back to billTotal. Example: if our bill 35.75 and we want to leave a 20% tip (0.2) our new billTotal should come out to 42.90.

// PUT YOUR CODE HERE

// Don't forget your console.logs!
let billTotal = 20.8;
let tipPercentage = 0.2;
let tip = billTotal * tipPercentage;
billTotal += tip;

console.log("Q12 The total will be: " + billTotal);

// ---------- QUESTION 13 ----------
// Create two variables named 'num1' and 'num2' and assign them integer values. Create a function called 'multiplyThese' that takes 2 parameters and returns the product  of the two parameters (as a reminder, a product is the resulting number when two numbers are multiplied together).

// EXAMPLE LOG:
//    console.log("Q13: ", multiplyThese(num1, num2));
// EXAMPLE OUTPUT: (if num1 and num2 are 2 and 5 respectively))
//    Q13: 10

// PUT YOUR CODE HERE
let num1 = 5;
let num2 = 10;

// Create the function to multiply the two numbers
function multiplyThese(a, b) {
  return a * b;
}

// Call the function with num1 and num2, and log the result
let result = multiplyThese(num1, num2);
console.log("Q13 The product of " + num1 + " and " + num2 + " is: " + result);

// ---------- QUESTION 14 ----------
// Building on the last question, create a function called 'getAverage' that takes 2 parameters and returns their average (hint: there is no built-in average operator in JavaScript).  Use the variables (num1 and num2) you created in Question 6 to test your function.  NOTE: In some programming languages, the types of numbers you use in equations can effect what type of number (integer/floating point) you get as a result.  We suggest using 2.0 instead of 2 as you're calculating the average.

// EXAMPLE LOG:
//    console.log("Q14: ", getAverage(num1, num2));
// EXAMPLE OUTPUT: (based on num1 and num2 above)
//    Q14: 3.5

// PUT YOUR CODE HERE
function getAverage(a, b) {
  return (a + b) / 2.0; // Ensure floating-point division
}

// Call the function with num1 and num2, and log the result
let average = getAverage(num1, num2);
console.log("Q14 The average of " + num1 + " and " + num2 + " is: " + average);
```
