# Week 4: JavaScript Array Methods — Group Mentor Guide

Welcome to Week 4 of the Intro to Programming course! This week, students are learning:

- How to use array methods like `forEach`, `map`, `filter`, and `find`
- What higher-order functions and callbacks are
- How to iterate through arrays in more powerful, expressive ways

Students are working in the `04-js-array-methods.js` assignment file.

## Warm-Up (5–10 minutes)

Choose one:

**Relationship-Building**  
- What’s a weird food combination you secretly enjoy?  
- What’s a skill or topic you’ve gotten really curious about recently?

**Check for Understanding (from last week)**  
- What’s an object, and how is it different from an array?  
- What does `this` refer to inside an object method?  
- How do you write a method inside an object?

## Explore vs. Apply — Session Formats

**Explore Sessions** → Walk through `forEach`, `map`, `filter`, and `find` with small examples  
**Apply Sessions** → Debug student code, remix array method usage, or create challenges together

## Sample Timing for 1-Hour Session

| Time      | Activity                                 |
|-----------|------------------------------------------|
| 0:00–0:10 | Warm-up + review last week               |
| 0:10–0:30 | Explore: walk through array method logic |
| 0:30–0:50 | Apply: live code + assignment help       |
| 0:50–1:00 | Wrap-up + final questions                |

## Check for Understanding (Ask 2–3)

- What’s a higher-order function?
- How is `map` different from `forEach`?
- What’s the purpose of a callback function?
- When would you use `filter` vs. `find`?

## Explore Prompts

Use these to demonstrate key concepts live:

- What’s a callback? Let’s write one by hand before using array methods.
- How does `map` create a new array? Let’s rewrite `addThreeToAll` together.
- What happens if `filter` doesn’t find any matches? What does it return?

*Mini-Demo Ideas:*  

    // .forEach example
    const names = ["Rosa", "Luis", "Amina"];
    names.forEach(function(name) {
      console.log("Hi " + name + "!");
    });

    // .map example
    const nums = [1, 2, 3];
    const doubled = nums.map(n => n * 2);
    console.log(doubled); // [2, 4, 6]

    // .filter example
    const mixed = [5, 10, 13, 18];
    const evens = mixed.filter(n => n % 2 === 0);
    console.log(evens); // [10, 18]

    // .find example
    const result = mixed.find(n => n > 12);
    console.log(result); // 13

---

## Apply Prompts (Live Coding & Troubleshooting)

### Assignment Hotspots
* Forgetting to `return` values in `map` or `filter` functions  
* Using `console.log()` inside `map()` when trying to return a new array  
* Reusing old variables instead of using function parameters  
* Confusing `filter` and `find` — they do very different things!  
* Misunderstanding how to access object properties in array methods (like `user.username`)

### Try This Live

**Let’s walk through Q10 together — how can we make a flexible `pluck` function?**

    function pluck(array, key) {
      return array.map(obj => obj[key]);
    }

Ask:
* What happens if the key doesn’t exist in one object?
* Can we rewrite this with a traditional `for` loop?

## Engagement Strategies (for quiet groups)

* Write & Remix: “Try Q7 with `.map()` — now try it again using `.forEach()` instead.”
* Fill in the Blank: “Here’s a broken `filter()` function — can you fix it?”
* Pair Code Review: “In pairs, compare your answers to Q13 — what’s different?”

## Optional Challenges

- Write your own `.map()` function from scratch using a `for` loop
- Add a `greeting` property to each user object using `.map()`
- Create your own mini `.filter()` to remove falsy values

## Mentor To-Do
- [ ] Run a session using this guide  
- [ ] Let students debug, explore, or build on their code  
- [ ] Submit your [Mentor Session Report](https://airtable.com/appoSRJMlXH9KvE6w/shrp0jjRtoMyTXRzh)
