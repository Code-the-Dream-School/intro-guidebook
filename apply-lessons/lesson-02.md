# Lesson 02: JavaScript Loops and Arrays
**Explore Lesson Plan**

**Learning objective:**

## Warm Up (5 minutes)

"Before we dive into loops and arrays, I'm curious - what's something repetitive you do in your daily life that you wish could be automated? Think about tasks you repeat over and over."
*(Allow 2-3 students to share briefly while taking attendance)*

## Direct Instruction (15-20 minutes)

### Intro to Loops (5-7 minutes)

  * Present slides 2-3: "Why Loop?" and "Types of Loops"
  * Emphasize the core purpose: automating repetitive tasks
  * Walk through each loop type with real-world analogies:
    * `for...of`: Like going through each item in your grocery bag
    * Standard `for`: Like counting down days until an event
    * `while`: Like continuing to study until you understand a concept
  * Address the "i" variable history from FORTRAN (slide 3)
  * Emphasize importance of meaningful variable names

### More Loops (5-7 minutes)

  * Present slides 4-6: "More Loops," "Break/Continue," and "Nested Loops"
  * Compare while vs do...while loops with examples
  * Explain break and continue using relatable scenarios:
      * `break`: Finding your keys and stopping the search
      * `continue`: Skipping a broken egg when cooking
  * Discuss nested loops with caution about performance implications
  * Point out real-world nested loops: days in weeks, hours in days

### Array Fundamentals (5-7 minutes)

  * Present slides 7-8: "Array Basics" and "Functional Programming"
  * Describe arrays as organized collections
  * Emphasize zero-indexing and accessing elements
  * Introduce functional methods with simple examples:
      * `map()`: Converting temperatures from F to C
      * `filter()`: Finding all prices under $20
      * `reduce()`: Calculating total cost of items
   
## Guided Practice (15-20 minutes)

### Breakout Room Activity: "Loop Challenges"

*Share a CodePen/JSFiddle link with these starter exercises.*

  * Tell studnets they will have about 15 minutes in breakout rooms to complete the task.
  * Use the breakout room feature to put students into small groups (around 3-5 students — whatever feels right depending on mentor session attendance and student engagement).
  * As students are in breakout rooms, feel free to cycle through the rooms to check in on students and answer questions. When entering a room, ask something like, "How’s it going? Any questions or roadblocks so far?"

#### 1. Basic Loop Practice 

```javascript
// 1. Write a for loop that prints numbers 1-10
// 2. Write a while loop that prints even numbers from 2-20
// 3. Use a for...of loop to print each fruit in the array
const fruits = ["apple", "banana", "cherry", "dragonfruit"];
```

#### 2. Break/Continue Challenge

```javascript
// 1. Print numbers 1-20, but skip any number divisible by 3
// 2. Find the first number between 1-100 that's divisible by both 7 and 11
```

#### 3. Array Methods Practice 

```javascript
const temperatures = [72, 68, 74, 77, 91, 65, 80, 72];
// 1. Use map() to convert these temperatures to Celsius
// 2. Use filter() to find all temperatures above 75
// 3. Use reduce() to find the average temperature
```

## Q&A and Wrap-Up (10 minutes)

#### Concept Review
  * "What was the most challenging concept we covered today?"
  * "Can anyone explain a real-world scenario where you'd use a nested loop?"
  * "When would you choose a while loop over a for loop?"

#### Reflection
  * "What's one thing from today's session that will help you with this week's coding assignment?"
  * "Any concepts you'd like to review in more depth?"

#### Preview
"In our Apply session, we'll use these loop and array concepts to build something practical. Before then, try experimenting with different loop types in your own code to see which feels most intuitive for different situations."

#### Resources to share: 
  * MDN documentation links for loops and array methods
  * Link to additional practice exercises
  * Remind about 1:1 mentor office hours for additional help
