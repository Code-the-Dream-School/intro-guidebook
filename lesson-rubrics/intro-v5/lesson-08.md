# Lesson 8: CSS Basics

| Week | Topic      | Learning Objective |
|------|------------|--------------------|
| 8  | CSS Basics | Students will be able to create and link an external CSS file; use selectors to style HTML elements; apply the CSS Box Model; and customize fonts, colors, spacing, and alignment.

## Assignment Rubric

You can mark the student's assignment as complete if they:

- [ ] Created a `css` folder and `index.css` file in the correct location
- [ ] Properly linked the CSS file in their HTML `<head>` section
- [ ] Successfully styled their portfolio with the minimum required changes (see checklist below)
- [ ] Used proper CSS syntax (selectors, properties, values, semicolons)
- [ ] Submitted their assignment via pull request

## Minimum Required Styling Changes

Students should have made **at least** these changes:

- [ ] Changed the background color of the page body
- [ ] Changed the default text color
- [ ] Customized at least one font family
- [ ] Added spacing (padding/margin) between sections
- [ ] Changed the alignment of content in at least one section
- [ ] Styled heading elements (font size, weight, and/or color)
- [ ] Transformed the style of their name at the top of the page
- [ ] Styled the "Experience" list items (could be blocks, colors, spacing, etc.)
- [ ] Styled the "Connect" links (color, hover effects, etc.)

## What to Look For

### CSS File Structure & Linking
```html
<!-- In index.html, should be in the <head> -->
<link rel="stylesheet" href="css/index.css">
```

### Proper CSS Syntax
```css
/* Good syntax examples */
body {
  background-color: #f5f5f5;
  color: #333333;
  font-family: Arial, sans-serif;
}

.section-title {
  font-size: 24px;
  margin-bottom: 15px;
}

#header {
  text-align: center;
  padding: 40px 0;
}
```

## Sample CSS Snippets (For Reference)

You don't need to provide these to students unless they ask, but here are some examples of what acceptable solutions might look like:

```css
/* Body styling */
body {
  background-color: #fafafa;
  color: #2c3e50;
  font-family: 'Helvetica', sans-serif;
  line-height: 1.6;
  margin: 0;
  padding: 20px;
}

/* Name/header styling */
#name {
  font-size: 48px;
  color: #2980b9;
  text-align: center;
  margin-bottom: 10px;
  font-weight: bold;
}

/* Section styling */
.section {
  background-color: white;
  padding: 30px;
  margin: 20px 0;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

/* Heading styling */
h2 {
  color: #34495e;
  font-size: 28px;
  border-bottom: 3px solid #3498db;
  padding-bottom: 10px;
  margin-top: 0;
}

/* List item styling */
.experience li {
  background-color: #ecf0f1;
  padding: 15px;
  margin: 10px 0;
  border-left: 4px solid #3498db;
}

/* Link styling */
a {
  color: #3498db;
  text-decoration: none;
  font-weight: bold;
}

a:hover {
  color: #2980b9;
  text-decoration: underline;
}
```

Remember: These are just examples. Student solutions will vary greatly, and that's a good thing!
