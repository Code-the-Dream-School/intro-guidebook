# Lesson 4.2 Teaching Notes 

| **Topic** | **Week** | **Class Website** |
| :---: | :---: | :---: |
| JavaScript and the DOM | 4.2 | [Link](https://learn.codethedream.org/dorado-js-and-dom/) |

## Outline 
- Overview
- Sample Mentor Session
- Common Issues

## Overview 

**Learning Objective:** Students will be able to create a JavaScript file in a project directory; add footer, copyright, and skills sections to their personal portfolio.

## Sample Mentor Session 

### :wave: Check-In

#### Check-In Open-Ended Questions 

- Start with an icebreaker from this [icebreaker list](https://docs.google.com/document/d/1WbwKn8B5GfRueq7Zbw0zx_k15aqyIqIs23i_WHI-pPI/edit?usp=sharing). 
- What is something that you are excited to learn more about this week? 

#### Check-In Progress Poll 

- What is your progress on **this week's** materials?

  - [ ] Done
  - [ ] Almost Done
  - [ ] Halfway
  - [ ] Just started
  - [ ] Haven't started

While students are responding to the check-in questions, take attendance. 

### :mag: Content Overview 

Let's review some key terms and concepts from this week's lesson materials: 

- DOM Overview
  - Node vs Element 
  - Selectors 
  - Altering and targeting DOM nodes
  - Nodelist vs. Array of nodes
  - Bubbling 
- Developer Tools 
  - View and change the DOM
  - Debug JavaScript
  - Use breakpoints
  - View the Resources Panel to check the scripts running on a website
  - Add CSS Pseudostate to a Class
  - View CSS Properties in Alphabetical Order
  - View and edit the Box Model of any Element in Chrome DevTools
  - View a page in print mode
  - Enable or Disable CSS Classes
  - Simulate media queries in Device Mode
- Understanding Errors
  - Syntax Errors
  - Reference Errors
  - Type Errors
  - Resolving Errors
 
### :notebook: Assignment Overview

TBD

### :thinking: Questions 

Use this time to answer students questions from the lesson materials and assignments. Rememember to incorporate teaching strategies: 

  - **Think aloud**: Narrate your thinking to show students how developers approach problems. For example, “When I saw this problem, I decided to approach it by…”
  - Use **positive narration**. For example, “I appreciate that Raheem has his camera on today” or “That was an excellent question."
  - **Warm call** on students or **practice popcorn calling** (students can ask another student for help) if participation is low.
  - Incorporate 10 seconds of **wait time** when you're expecting students to respond to you. This is how long it takes the average person to formulate their answer to your question or think of a question of their own. 


### :telescope: Looking Ahead 

Next week, students will practice more with the DOM and add a form to their portfolio project. 

### :nerd_face: Mentor Session Report Form 

Please remember to fill out the [Mentor Session Report Form](https://airtable.com/shrp0jjRtoMyTXRzh) at the end of the session.

## :100: Assignment Rubric 
[Assignment](https://github.com/Code-the-Dream-School/intro-to-programming-dorado/blob/main/instructions/section-4/lesson-4-2.md)

Check the student has created a PR to submit their assignment:
- [ ] [Created a PR](https://github.com/Code-the-Dream-School/intro-to-programming-dorado/blob/main/instructions/common/how-to-pull-request.md)

Check student's repository for:
- [ ] Created an `index.js` file
- [ ] Updated `index.html` file
  - [ ] Linked the `js` file with a `<script>` tag at the bottom of the `<body>`
  - [ ] Added an empty `<footer>` tag at the bottom of the `<body>`
  - [ ] Above the `Connect` section, added `<section>` tag with an id of `skill`
  - [ ] Inside the skill `<section>`, added `<h2>` with content `Skills`
  - [ ] Inside the skill `<section>`, added an empty `<ul>`
- [ ] Dynamically add a copy right footer using `index.js`
  - [ ] Store Date in var `today`
  - [ ] Store current year in var `thisYear`
  - [ ] Store footer element in var `footer` (using DOM Selection)
  - [ ] Create new `p` element and store in var `copyright`
  - [ ] Set innerHtml of `copyright` to the student's name and current year
  - [ ] Append the `copyright` paragraph the `footer` element (using DOM Manipulation)
- [ ] Dynamically add skills using `index.js`
  - [ ] Create a list var `skills` that contains the student's skills
  - [ ] Select `#skills` section and store in var `skillsSection` (using DOM Selection)
  - [ ] Create a `for loop` to iterate of the `skills` variable
  - [ ] Inside loop, create a `<li>` element in var `skill` for each skill and set the innerHtml of `skill` to the current value in the loop
  - [ ] Inside loop, append the `skill` variable to the `skillsList` element


## Common Issues 

TBD
