# Week 8: CSS Basics — Group Mentor Guide

Welcome to Week 8 of the Intro to Programming course! This week, students are learning:

- What CSS is and how it styles HTML pages
- How to link external stylesheets
- How to use selectors (element, class, and ID)
- The CSS Box Model (margin, border, padding, content)
- Basic styling properties (colors, fonts, spacing, alignment)

Students are working on styling their personal portfolio page with `index.css`.

## Warm-Up (5–10 minutes)

Choose one:

**Relationship-Building**  
- What's a website you think looks really good? What makes it stand out?  
- If you could change one thing about how a website you use daily looks, what would it be?

**Check for Understanding (from HTML week)**  
- What's the difference between a `<div>` and a `<section>`?  
- When should you use semantic HTML elements?  
- How do you make a link open in a new tab?

## Explore vs. Apply — Session Formats

**Explore Sessions** → Walk through CSS syntax, selectors, and the box model with live examples  
**Apply Sessions** → Debug student CSS, experiment with styling together, or remix their portfolio designs

## Sample Timing for 1-Hour Session

| Time      | Activity                                 |
|-----------|------------------------------------------|
| 0:00–0:10 | Warm-up + review HTML structure          |
| 0:10–0:30 | Explore: CSS syntax, selectors, box model|
| 0:30–0:50 | Apply: live styling + troubleshooting    |
| 0:50–1:00 | Wrap-up + final questions                |

## Check for Understanding (Ask 2–3)

- How do you link a CSS file to an HTML file?
- What's the difference between a class and an ID selector?
- What's the CSS Box Model? What's the order from outside to inside?
- What's the difference between `margin` and `padding`?
- How do you change the background color vs. the text color?

## Explore Prompts

Use these to demonstrate key concepts live:

- Let's link a CSS file to HTML — what goes in the `<head>`?
- How do selectors work? Let's try styling all `<p>` tags, then just one with a class.
- What happens when we add a border? Let's explore the box model together.

*Mini-Demo Ideas:*  

```css
/* Element selector - styles ALL paragraphs */
p {
  color: blue;
  font-size: 18px;
}

/* Class selector - styles elements with class="intro" */
.intro {
  background-color: lightgray;
  padding: 20px;
}

/* ID selector - styles the element with id="header" */
#header {
  text-align: center;
  margin-bottom: 30px;
}

/* Box Model demonstration */
.box-example {
  width: 200px;
  padding: 20px;      /* space inside */
  border: 2px solid black;
  margin: 10px;       /* space outside */
}
```

---

## Apply Prompts (Live Coding & Troubleshooting)

### Assignment Hotspots
* Forgetting to link the CSS file or using the wrong file path  
* Confusing classes (`.classname`) with IDs (`#idname`)  
* Not seeing changes because the browser cached old CSS  
* Mixing up `margin` and `padding`  
* Forgetting units on values (writing `padding: 20` instead of `padding: 20px`)
* Accidentally styling the wrong elements due to selector mistakes
* Spelling errors in property names or values

### Try This Live

**Let's style a section together using the box model:**

```css
.experience {
  background-color: #f0f0f0;
  padding: 25px;           /* space inside the section */
  margin: 20px 0;          /* space above and below */
  border-left: 4px solid #0066cc;
}

.experience h2 {
  color: #0066cc;
  margin-top: 0;           /* remove default top margin */
}
```

Ask:
* What happens if we change `padding` to `margin`?
* How can we add space just on the left side?
* What if we want different colors for different sections?

## Engagement Strategies (for quiet groups)

* Before & After: "Let's take one section and transform it together — what should we change first?"
* Remix Challenge: "Pick a classmate's portfolio and suggest one CSS improvement to try."
* Debug This: "Here's CSS that isn't working — can you spot the error?"
* Color Picker Fun: "Let's find three colors that work well together for your portfolio."

## Optional Challenges

- Use Google Fonts to add a custom font to your page
- Create a hover effect that changes link colors
- Add a border to just one side of an element
- Use `text-align`, `margin`, and `padding` to center content
- Experiment with `border-radius` to make rounded corners

## Common Questions & Answers

**Q: My CSS isn't showing up!**  
A: Check that your `<link>` tag is in the `<head>` and the file path is correct. Try hard-refreshing (Ctrl+Shift+R or Cmd+Shift+R).

**Q: When should I use a class vs. an ID?**  
A: Use classes for styling multiple elements the same way. Use IDs for unique elements you'll only have one of.

**Q: Why is there space around my elements I didn't add?**  
A: Browsers add default margins and padding to elements. You can override them with CSS.

## Mentor To-Do
- [ ] Run a session using this guide  
- [ ] Encourage creative experimentation with styling  
- [ ] Submit your [Mentor Session Report](https://airtable.com/appoSRJMlXH9KvE6w/shrp0jjRtoMyTXRzh)
