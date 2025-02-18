# Lesson 02: JavaScript Loops and Arrays
**Explore Lesson Plan**

**Learning objective:** Students will be able to construct efficient solutions to repetitive tasks by designing and implementing loops, particularly 'for' loops, while avoiding common pitfalls such as infinite loops; analyze and manipulate arrays to effectively organize and access data.

## Warm Up (5 minutes)

"Let's review what we learned in our Explore session. Can someone explain why loops are important in programming? What types of problems do they help us solve?"
*Allow 2-3 students to share while taking attendance*

## Direct Instruction: Assignment Overview (5-7 minutes)

### Assignment Review:

  * Share screen to show the assignment page
  * Explain structure: 13 questions covering loops, arrays, and array methods
  * Review expectations:
      * All functions need console.log verification
      * Testing with multiple inputs is encouraged
      * Code should be well-commented

### "I Do" Demo: Approaching a Loop Problem (using Q1 as example)

  * Walk through reading and understanding the problem statement
  * Demonstrate planning process: "We need to repeat an action n times"
  * Code the solution step-by-step with narration:

```javascript
function repeat(times) {
  // Initialize a loop that runs 'times' number of iterations 
  for (let i = 0; i < times; i++) {
    // Each iteration, print "Hello World!"
    console.log("Hello World!");
  }
}

// Test the function
repeat(3);
```

  * Explain the structure: function declaration, loop setup, action inside loop
  * Show execution flow step-by-step

## Guided Practice: "We Do" (15-20 minutes)

### Collaborative Coding: Question 2 & 3

  * Share screen and invite student participation
  * For Q2 (pyramidCounting):
      * Ask: "What's our approach for adding numbers from 0 to n?"
      * Guide students to suggest loop structure
      * Develop solution together:

```javascript
function pyramidCounting(num) {
  let sum = 0;
  for (let i = 0; i <= num; i++) {
    sum += i;
  }
  return sum;
}

console.log("Q2: ", pyramidCounting(4));
```

  * For Q3 (noVowels):
      * Ask: "How can we identify vowels in a string?"
      * Have students suggest approaches for removing characters
      * Build solution together:
   
   ```javascript
function noVowels(str) {
  const vowels = "aeiouAEIOU";
  let result = "";
  
  for (let i = 0; i < str.length; i++) {
    if (!vowels.includes(str[i])) {
      result += str[i];
    }
  }
  
  return result;
}

console.log("Q3: ", noVowels("adventurous"));
```

* Discuss alternative approaches (while loops, different vowel checks)

## Independent Practice "You Do" (15-20 minutes)

### Breakout Room Challenges

  * Divide students into breakout rooms (3-4 students per room)
  * Assign specific questions based on complexity:
    * Group 1: Q4 (vowelCount) and Q5 (numOfOdds)
    * Group 2: Q6 (arrayChecker) and Q7 (getElementAt)
    * Group 3: Q8 (insertInArray) and Q9 (compareArrays)
    * Group 4: Q10 (calculateTotal)
  * Provide hints for each question in a shared document:
    * Q4: "Consider using a counter variable and a loop to check each character"
    * Q5: "Remember the modulo operator checks for remainders"
    * Q6: "How can you check if an array has any elements?"
    * Etc.
  * Instruct students to:
    * Work collaboratively
    * Test solutions with multiple inputs
    * Be prepared to share their approach
   
 *Monitor breakout rooms and provide assistance where needed*

 ## Wrap-Up and Q&A (10-15 minutes)
 ### Solutions Review
   * Have one representative from each group share their approach for one question
   * Discuss alternative solutions and optimizations
   * Address common errors or misconceptions

### Advanced Array Methods Preview:
  * Briefly demonstrate one "stretch goal" solution using array methods:

```javascript
// Q10 stretch goal with reduce()
function calculateTotal2(numbers) {
  return numbers.reduce((sum, current) => sum + current, 0);
}
```

  * Explain benefits: readability, fewer bugs, declarative style

### Assignment Tips:
  * "Start with the problems that seem most straightforward"
  * "Test your functions with multiple inputs"
  * "Remember to check if your loop conditions handle edge cases"
  * "Use meaningful variable names to make your code more readable"

### Questions and Support

  * Address remaining questions
  * Remind students of office hours and support resources
  * Encourage peer collaboration (while maintaining academic integrity)

### Closing
"Before our next session, try to complete at least questions 1-8. If you get stuck, write comments explaining your thought process - that will help us provide better guidance. Remember that mastering loops and arrays is fundamental to becoming a strong JavaScript developer!"
