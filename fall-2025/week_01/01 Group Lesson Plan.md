# Lesson Plan 01 – JS Basics & Functions

## About This Week
This week introduces students to the JavaScript language and its role in web development.
Students learn fundamental syntax, variables, data types, conditionals, and basic functions through the Odin Project and Scrimba modules.
By the end of the week, students should be able to write and call simple functions, use variables correctly, and debug using the console.
The coding assignment asks them to practice these skills through short, incremental tasks that build confidence with core concepts.

---

## Explore Session (60 minutes)

**Purpose:** Reinforce the week’s lesson content and build comfort using JavaScript syntax before students begin the assignment.  
**Materials:** Mentor slides (Explore section), code editor or Scrimba demo, chat or polls for participation.

### Segment 1 – Warm-Up (5 min)
- Ask: “What’s one thing you already know—or think you know—about JavaScript?”  
- Quick poll or chat question: “Where does JavaScript run—browser, server, or both?”  
*Mentor Tip: Keep the tone low-stakes and inclusive; any answer that invites follow-up is useful.*

---

### Segment 2 – I Do (10 min)
Mentor demonstrates the basics:
```js
let firstName = "Jazmine";
let age = 27;
console.log("Hello, my name is " + firstName);
```
Explain:
- What a variable is and how `let` or `const` declares it  
- Difference between strings, numbers, and booleans  
- How `console.log()` helps test code  

**CFU Questions**
- “What happens if we forget quotation marks around a string?”  
- “What’s the difference between declaring and assigning a variable?”  

*Mentor Tip: Type live, narrating each small decision to model debugging habits.*

---

### Segment 3 – We Do (20 min)
Collaborative example: build a simple function together.
```js
function greet(name) {
  return `Hello, ${name}!`;
}
console.log(greet("Luis"));
```
Discuss:
- Function declaration vs function call  
- Parameters and return values  
- Arrow-function shorthand (briefly)  

Invite students to suggest small changes (e.g., add another parameter for time of day).  
**CFU Questions**
- “What happens if a function doesn’t have a return statement?”  
- “How could we test this with a different input?”  

---

### Segment 4 – You Do (20 min)
Students try a short task in pairs or chat:
> “Write a function `double(num)` that returns twice the input number.  
> Share your output in chat.”

Mentor walks through one or two solutions, emphasizing syntax and logic rather than perfection.

---

### Segment 5 – Wrap-Up (5 min)
- Summarize key takeaways: variables → conditionals → functions.  
- Ask: “What’s one thing you’ll practice before the Apply session?”  
- Remind students to review Scrimba’s *JS Deep Dive – Functions* before next time.  

---

## Apply Session (60 minutes)

**Purpose:** Support students as they complete the Week 1 assignment, practicing problem-solving and debugging.  
**Materials:** Mentor slides (Apply section), assignment file (Questions 1–15), code editor, breakout rooms optional.

### Segment 1 – Quick Recap (5 min)
- Ask: “What new thing did you try in your code this week?”  
- Address common issues from Slack or office-hour questions (e.g., forgetting to remove `//` from console logs).

---

### Segment 2 – Guided Coding (25 min)
Mentor demonstrates solving one representative problem (e.g., Question 12 – `messageString`):
```js
function messageString() {
  return "Welcome to Code the Dream";
}
console.log(messageString());
```
Talk through reading instructions carefully, testing outputs, and comparing expected vs actual results.

**CFU Questions**
- “How can we tell if our function actually returned a value?”  
- “What error message might we see if a variable isn’t declared?”  

*Mentor Tip: Keep your console visible—model iterative testing rather than finished code.*

---

### Segment 3 – Peer or Solo Debugging (20 min)
- Invite students to share a line of code they’re stuck on.  
- Screen-share one or two examples; troubleshoot together.  
- Highlight patterns of common bugs (missing braces, case sensitivity, incorrect returns).  

Encourage students to verbalize what they tried and what they’ll try next.

---

### Segment 4 – Wrap-Up and Reflection (10 min)
Discussion or chat prompt:
> “What’s one bug you solved today and how did you find the fix?”  
> “What’s one strategy you’ll use when you get stuck next time?”

Remind students:
- Assignments are due before the next Monday.  
- It’s okay to ask for help early—share your question with code snippets and error messages.

*Mentor Tip: End with encouragement. Many students run their first working JS function this week—celebrate that milestone.*

---

### Notes for Mentors
- Maintain consistent pacing; aim for variety—talking, demoing, practicing.  
- Model curiosity over perfection; let small syntax mistakes become teaching moments.  
- Encourage chat participation if cameras are off.  
- Reinforce that errors are expected and valuable learning opportunities.
