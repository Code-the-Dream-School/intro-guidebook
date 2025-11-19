# Week 2: Loops & Arrays — Group Mentor Guide

Welcome to Week 2 of the Intro to Programming course! This week, students learned about:

- Using `for` and `while` loops for repetition
- Creating and manipulating arrays
- Looping through arrays and understanding how to access or modify data

Students are working in the `02-loops-and-arrays.js` assignment file.

## Warm-Up (5–10 minutes)

Choose one:

**Relationship-Building**
- What’s your favorite app or website, and why?
- If you could automate one part of your life with code, what would it be?

**Check for Understanding (from last week)**
- What does `console.log()` do?
- What are some ways we can define a variable in JavaScript?
- What’s the difference between calling a function and defining one?

## Explore vs. Apply — Session Formats

**Explore Sessions** → Talk through concepts, whiteboard examples, or live code walk-throughs  
**Apply Sessions** → Debug code, work through problems together, or remix code for new outputs

Mix and match based on student needs!

## Sample Timing for 1-Hour Session

| Time      | Activity                            |
|-----------|-------------------------------------|
| 0:00–0:10 | Warm-up + review last week          |
| 0:10–0:30 | Explore: discuss loops and arrays   |
| 0:30–0:50 | Apply: live code + assignment help  |
| 0:50–1:00 | Wrap-up + final questions           |

## Check for Understanding (Ask 2–3)

- What’s the difference between a `for` loop and a `while` loop?
- What do arrays let us do that variables can’t?
- What does `array[i]` give us?

## Explore Prompts

Use these prompts to drive discussion:

- Can anyone explain what a loop is *without* using the word “loop”?
- Let’s draw out how `i++` changes with each iteration — what happens if we forget to update it?
- Arrays are like shelves — how can we describe how we access or change a value on one “shelf”?

*Mini-Demo:*  
```js
// What's wrong with this loop?
for (let i = 0; i < 5; ) {
  console.log("Infinite?");
}
```
## Apply Prompts (Live Coding & Troubleshooting)

### Assignment Hotspots
* Students accidentally log *inside* vs *outside* functions
* Forgetting to return a value from a function
* `undefined` from missing return or incorrect index

## Try This Live

“Let’s walk through Q3 together — how can we loop through a string and remove vowels?”

```js
function noVowels(str) {
  let result = "";
  for (let i = 0; i < str.length; i++) {
    let char = str[i].toLowerCase();
    if (!"aeiou".includes(char)) {
      result += str[i];
    }
  }
  return result;
}

console.log("Test:", noVowels("adventurous"));
```

Ask:
* What would happen if we used `continue` instead of `if`?
* Can we rewrite this with `.split()` and `.filter()`?

## Engagement Strategies
* Chat First: “Type your answer in chat first, then unmute to share.”
* Two-Minute Pairing: “Find a partner and compare your versions of Q2 — how are they different?”
* Explain My Bug: Show a broken loop and ask, “What do you think this code is trying to do?”

## Optional Challenges
* Rewrite Q10 using `reduce()`
* Modify Q13’s `fizzBuzz` to return an object with counts of “fizz”, “buzz”, and “fizzbuzz”
* Create your own version of `makeSquares` using `map()`

## Mentor To-Do
- [ ] Run a session using this guide
- [ ] Let students debug, explore, or build on their code
- [ ] Submit your [Mentor Session Report](https://airtable.com/appoSRJMlXH9KvE6w/shrp0jjRtoMyTXRzh)
