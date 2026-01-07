# Week 9: HTML Basics – Group Mentor Guide

Welcome to Week 9 of the Intro to Programming course! This week, students are learning:

- The history and structure of the web
- HTML syntax, including elements, tags, and attributes
- How to create basic page structure with boilerplate HTML
- Semantic HTML elements like `<section>`, headings, paragraphs, and lists
- Working with links and file paths
- Basic form elements and web accessibility

Students are working on creating a portfolio page in their `index.html` file.

## Warm-Up (5–10 minutes)

Choose one:

**Relationship-Building**  
- What's a website you visit every day? What keeps you coming back?
- If you could redesign any website, which would it be and why?

**Check for Understanding (from last week)**  
- What's a higher-order function?
- How is `map` different from `forEach`?
- When would you use `filter` vs `find`?

## Explore vs. Apply – Session Formats

**Explore Sessions** → Walk through HTML structure, demonstrate tags and elements live  
**Apply Sessions** → Debug student HTML, review their portfolio pages, troubleshoot syntax errors

## Sample Timing for 1-Hour Session

| Time      | Activity                                 |
|-----------|------------------------------------------|
| 0:00–0:10 | Warm-up + review last week               |
| 0:10–0:30 | Explore: walk through HTML fundamentals  |
| 0:30–0:50 | Apply: live code + assignment help       |
| 0:50–1:00 | Wrap-up + final questions                |

## Check for Understanding (Ask 2–3)

- What's the difference between a tag and an element?
- Why do we need both opening and closing tags?
- What goes in the `<head>` vs the `<body>`?
- What's a semantic HTML element? Can you give an example?
- What's the difference between `<ul>` and `<ol>`?

## Explore Prompts

Use these to demonstrate key concepts live:

- Let's write boilerplate HTML from scratch together – what does each part do?
- How do we structure content with headings and paragraphs?
- What's the difference between inline and block-level elements?

*Mini-Demo Ideas:*  

```html
<!-- Basic structure -->
<!DOCTYPE html>
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <h1>Welcome!</h1>
    <p>This is my page.</p>
  </body>
</html>

<!-- Semantic sections -->
<section id="about">
  <h2>About Me</h2>
  <p>I'm learning to code!</p>
</section>

<!-- Lists -->
<ul>
  <li>JavaScript</li>
  <li>HTML</li>
  <li>CSS</li>
</ul>

<!-- Links -->
<a href="https://github.com/username">My GitHub</a>
```

---

## Apply Prompts (Live Coding & Troubleshooting)

### Assignment Hotspots
* Forgetting closing tags (especially `</section>` or `</ul>`)
* Mixing up `<head>` and `<body>` content
* Not including required boilerplate elements (`<!DOCTYPE>`, `<html>`, `<head>`, `<body>`)
* Incorrect nesting – elements not properly contained within their parents
* Missing `id` attributes on sections
* Confusing `<ul>` (unordered) with `<ol>` (ordered) lists
* Not wrapping list items in `<li>` tags
* Missing `href` attribute in `<a>` tags

### Try This Live

**Let's build a section together – what makes it semantic?**

```html
<section id="experience">
  <h2>Experience</h2>
  <ul>
    <li>JavaScript fundamentals</li>
    <li>Array methods</li>
    <li>HTML structure</li>
  </ul>
</section>
```

Ask:
* Why use `<section>` instead of `<div>`?
* What's the purpose of the `id` attribute?
* How does proper nesting help the browser understand our page?

## Engagement Strategies (for quiet groups)

* **Show and Tell:** "Open your HTML file in a browser – what do you see?"
* **Spot the Error:** Share a broken HTML snippet and have students identify the issue
* **Build Together:** "Let's all add a new section to our pages at the same time"
* **Compare Approaches:** "What different ways can we structure a list of links?"

## Optional Challenges

- Add an image to your About section using `<img>` tag
- Create a navigation menu with links to each section using `<nav>`
- Add more metadata to your `<head>` (description, keywords, viewport)
- Include a footer with copyright information

## Mentor To-Do
- [ ] Run a session using this guide  
- [ ] Help students view their HTML pages in a browser
- [ ] Encourage students to experiment with different HTML elements
- [ ] Submit your [Mentor Session Report](https://airtable.com/appoSRJMlXH9KvE6w/shrp0jjRtoMyTXRzh)
