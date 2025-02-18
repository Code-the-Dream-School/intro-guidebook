# Lesson 01: JavaScript Basics and Functions
**Apply Lesson Plan**

**Learning objective:** Students will develop the ability to apply foundational JavaScript concepts, including variables, data types, conditional statements, and functions, to create and troubleshoot basic programs; evaluate the use of arrow functions and traditional functions to understand their syntax, benefits, and appropriate use cases.

Links: 
  * [Lesson content](https://classes.codethedream.org/course/intro-to-programming-v5/kepler?week=2&lesson=JavaScript+Loops+and+Arrays)
  * [Assignment content](https://codesandbox.io/p/sandbox/lesson-2-javascript-loops-and-arrays-2025-wzp3tj)
  * [Explore slides](https://github.com/Code-the-Dream-School/intro-guidebook/blob/main/group-session-slides/CTD%20Intro%20Week%202.pdf)

## Warm Up (5 minutes)

"Let's quickly remind ourselves how a function works by looking at a simple example:"

```javascript
// Function declaration
function combineStrings(string1, string2) {
  return string1 + " " + string2;
}

// Function call with arguments
console.log(combineStrings("Hello", "World"));
console.log(combineStrings("JavaScript", "Functions"));
```

"Today we'll be extending these function skills by combining them with loops and arrays to solve more complex problems."

## Direct Instruction: Assignment Overview (5-7 minutes)

### Assignment Structure
  * Share screen showing the assignment document
  * Explain the organization: 15 questions covering variables, data types, conditionals, and functions
  * Point out the commented console logs that need to be uncommented
  * Demonstrate where to check output in the console

### "I Do" Demo: Question Setup & Console Logs

  * Walk through how to read the instructions
  * Demonstrate establishing variables with proper camel case naming:

```javascript
let firstName = "Maria";
let lastName = "Rodriguez";
let country = "Mexico";

console.log("Q1: My first name is: ", firstName);
console.log("Q1: My last name is: ", lastName);
console.log("Q1: I was born in the country: ", country);
```

  * Show console output and explain how to verify results
  * Point out common issues (forgetting quotes for strings, syntax errors)

## Guided Practice: "We Do" (15-20 minutes)

### Collaborative Coding: Questions 2 & 4

For Q2 (Numerical Variables):

  * Ask: "What types of numbers do we need to create?"
  * Guide students through defining each variable type:

```javascript
let floatingPoint = 42.7531;
let integer = 15;
let negative = -8;
let notANumber = 4 * "hello";

console.log("Q2: This is a decimal, also called a floating point number: ", floatingPoint);
console.log("Q2: This is a whole number, also called an integer: ", integer);
console.log("Q2: This is a negative number: ", negative);
console.log("Q2: You can't multiply 4 by a word! ", notANumber);
```

  * Discuss what happens with the notANumber variable and why
  * For stretch goal, try a big number and observe behavior

For Q4 (String Concatenation):

  * Ask: "How can we combine our name variables from Q1?"
  * Develop two approaches together:

```javascript
// Standard concatenation
let fullIntroduction = "Hello! My name is " + firstName + " " + lastName + " and I was born in " + country;
console.log("Q4: Using concatenation: ", fullIntroduction);

// Stretch goal: Template literals
let templateIntroduction = `Hello! My name is ${firstName} ${lastName} and I was born in ${country}`;
console.log("Q4: Using template literals: ", templateIntroduction);
```

  * Compare both approaches and discuss advantages of template literals

## Independent Practice: "You Do" (20-25 minutes)

### Breakout Room Challenge: 

  * Divide students into breakout rooms (3-4 students per room)
  * Assign questions based on complexity:
    * Group 1: Q5 (Number Addition) and Q6 (String Methods)
    * Group 2: Q7 (Conditional) and Q8 (Age Conditional)
    * Group 3: Q9 (Random Number Generator) and Q10 (Number Rounding)
    * Group 4: Q12 (Basic Function) and Q13 (Function with Variables)
  * Provide helpful tips in a shared document:
      * For string methods: "Remember to check the MDN documentation for string methods"
      * For conditionals: "Make sure your comparison operators match what you're trying to test"
      * For functions: "Remember that functions need a return statement to output a value"
  * Instructions for students:
    * Work together to solve the problems
    * Test solutions with console.logs
    * Be prepared to present one solution to the whole group
    * Try the stretch goals if time permits

*Monitor breakout rooms and provide assistance as needed*

## Demo & Code Review (15 minutes)

### Group Solution Sharing:
  * Have one representative from each group share their screen and explain their solution
  * Encourage questions and alternative approaches
  * Address common mistakes or misconceptions

### Function Focus (Q14 & Q15):
  * Highlight the transition to parameter-based functions:

```javascript
// Q14: Function with one parameter
function useParams(word) {
  return word.toUpperCase();
}
console.log("Q14: ", useParams("hello"));
console.log("Q14: ", useParams("javascript"));

// Q15: Function with two parameters
function biggestStringLength(word1, word2) {
  if (word1.length >= word2.length) {
    return word1.length;
  } else {
    return word2.length;
  }
}

let word1 = "programming";
let word2 = "code";
console.log("Q15: ", biggestStringLength(word1, word2));
```

  * Discuss function structure: declaration, parameters, body, return statement
  * Show alternative approaches (ternary operator, Math.max)
  * Demonstrate edge cases (empty strings, null values)

## Wrap-Up and Q&A (5-10 minutes)
### Assignment Tips:
  * "Start with the questions you find easiest"
  * "Use descriptive variable names, even if the instructions don't require it"
  * "Test your code with different values"
  * "Comment your code to explain your thought process"

### Debugging Strategies:
  * Check for syntax errors (missing semicolons, quotes, brackets)
  * Verify variable types with `typeof`
  * Use console.log to trace variable values
  * Read error messages carefully

Support Resources:
  * Remind about 1:1 mentor office hours and mentoring availability
  * Share helpful documentation links (MDN, W3Schools)
  * Encourage peer collaboration while respecting academic integrity

### Closing
"For next week, try to complete all 15 questions. Focus on understanding the concepts rather than just getting the right answer. If you get stuck, add comments explaining what you're trying to do and what's confusing you. This will help us provide better guidance. Function parameters will be especially important as we move into loops and arrays next week!"
