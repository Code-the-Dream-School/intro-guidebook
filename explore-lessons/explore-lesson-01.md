# Lesson 01: JavaScript Basics and Functions

**Weekly Learning objective**

Students will develop the ability to apply foundational JavaScript concepts, including variables, data types, conditional statements, and functions, to create and troubleshoot basic programs; evaluate the use of arrow functions and traditional functions to understand their syntax, benefits, and appropriate use cases.

*Note:* This week, we'll focus on data types and conditional statements in the "Explore" lesson and writing JavaScript functions in the "Apply" lesson. 

**Lesson resources**

* Explore lesson slides
* Coding assignment rubric

## Lesson Plan

### Entrance ticket (~5 minutes)

**Display the first slide:**

  * **Discussion Prompt**: Welcome to the first week of this class! What made you interested in code? Write your answer in chat or share aloud.
      * Note thoughtful student responses and encourage participation in the chat if students are quiet.
      * Feel free to share why you became interested in code as well!

**Display the second slide to show the learning objective.**

### Part 1: Mentor-led instruction (~15 minutes)

**Display the Mentor-led instruction slides.**

  * Overview of JavaScript Data types: 
      * Primitive types: `string`, `number`, `boolean`, `undefined`, `null`, `symbol`, `bigint`
      * Non-primitive type: `object`
  * Use examples:

```js
let name = "Jazmine"; // string
let age = 25;         // number
let isStudent = true; // boolean
let score;            // undefined
let emptyValue = null; // null
let user = {name: "Jazmine", age: 25}; // object
```

  * Discuss type checking using `typeof`

**Display the activity slides.**

  * Interactive activity
      * Show the lines of code on teh slide and ask students to identify the data types:
      * Teacher notes:
   
```js
const weather = "sunny"; // string
const temperature = 72; // number
const isRaining = false; // boolean
```

### Part 2: Guided practice (~15 minutes)

**Switch to the Guided Practice slides.**

  * Introduce conditional logic:
      * `if`, `else if`, and `else` statements.
      * `switch` statements
  * Example:

```.js
const age = 20;

if (age < 18) {
  console.log("Minor");
} else if (age < 65) {
  console.log("Adult");
} else {
  console.log("Senior");
}
```

  * Walk through the following sample problem with the class:

      * Write a conditional statement that determines whether a number is positive, negative, or zero."

  **Switch to your IDE and "think aloud" with the students, explaining why are you are makign certain choices as you write the conditional.**

  * Example solution:  

```js
const number = -5;

if (number > 0) {
  console.log("Positive");
} else if (number < 0) {
  console.log("Negative");
} else {
  console.log("Zero");
}
```

### Part 3: Independent practice (~15 minutes)

**Share screen with the small group practice instructions slide.**

  * Give students the following instructions:
    * "We're now going to practice debugging a conditional statement in small groups. On the screen and in the chat is a conditional statement that is broken.
    * Why do you think it is broken? Work in your small groups to find the answer, and be ready with an explanation."
  * Tell studnets they will have about 5 minutes in breakout rooms to complete the task.
  * Use the breakout room feature to put students into small groups (around 3-5 students — whatever feels right depending on mentor session attendance and student engagement).
  * As students are in breakout rooms, feel free to cycle through the rooms to check in on students and answer questions. When entering a room, ask something like, "How’s it going? Any questions or roadblocks so far?"

Bugged code: 

```js
const temperature = 85;

if temperature > 80 {
  console.log("Hot");
} else {
  console.log("Cool");
}
```

Debugged code: 

```js
if (temperature > 80) {
  console.log("Hot");
} else {
  console.log("Cool");
}
```

  * After about 10 minutes, bring students back to the main call.
     * Ask, "What was one challenge you encountered in your small group? How were you able to overcome it?"
     * For shy or quiet groups, suggest using targeted questions (e.g., “What’s one thing that stood out to you about versioning systems?”).
     * For highly engaged groups, mentors could encourage deeper discussion or additional practice.
  * Finish the discussion by celebrating students' hard work.

### Exit Ticket (~5 minutes)

  * As the session wraps up, explain to students that they will write some basic JavaScript functions in this week's "Apply" lesson.
  * Stay on the call for a few minutes for any Q&A. 
