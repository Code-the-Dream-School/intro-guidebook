# Lesson 7: HTML Basics - Assignment Review Guide

| Week | Topic       | Learning Objective |
|------|-------------|--------------------|
| 7    | HTML Basics | Students will be able to write HTML boilerplate code from scratch, structure page content using semantic HTML elements, and create a basic portfolio page with sections, lists, and links.

## Assignment Rubric

You can mark the student's assignment as complete if they:

- [ ] Have created a new branch (`lesson-7`) and submitted a pull request
- [ ] Include proper HTML boilerplate written from scratch (DOCTYPE, html, head, body tags)
- [ ] Have a `<title>` element in the `<head>`
- [ ] Include at least two `<meta>` elements in the `<head>`
- [ ] All visible content is inside `<body>` tags
- [ ] Include the following content in order:
  - Name in an `<h1>` element
  - Three sections: About, Experience, and Connect
  - Each section wrapped in a `<section>` element with an `id` attribute
  - Each section has an `<h2>` heading
  - About section has a `<p>` paragraph
  - Experience section has a `<ul>` with at least one `<li>` item
  - Connect section has at least two `<a>` links (GitHub and LinkedIn minimum)
- [ ] All tags are properly nested and closed
- [ ] Use proper HTML syntax throughout

## Common Issues to Watch For

### Structure Issues
* **Missing DOCTYPE:** Should be `<!DOCTYPE html>` on line 1
* **Unclosed tags:** Every opening tag needs a closing tag (except self-closing tags like `<meta>`)
* **Improper nesting:** Elements should be fully contained within their parent elements
* **Content outside `<body>`:** All visible content must be inside `<body>` tags

### Head Section
* **Missing or incorrect `<title>`:** Should describe the page (e.g., "Maria Santiago's Portfolio")
* **Not enough meta tags:** Should have at least two (could include charset, viewport, description, keywords, author)
* **Meta tags not self-closing:** Should end with `/>` like `<meta charset="UTF-8" />`

### Body Content
* **Missing section wrappers:** Each of the three sections should be wrapped in `<section>` tags
* **Missing `id` attributes:** Each section should have an `id` matching its content (e.g., `<section id="about">`)
* **Wrong heading levels:** Should use `<h1>` for name, `<h2>` for section titles
* **Lists not properly structured:** `<ul>` should contain `<li>` elements, not bare text
* **Links missing `href`:** `<a>` tags need `href="url"` to work properly

## Sample Correct Code Structure

```html
<!DOCTYPE html>
<html>
  <head>
    <title>John Doe's Portfolio</title>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  </head>
  <body>
    <h1>John Doe</h1>
    
    <section id="about">
      <h2>About</h2>
      <p>I'm a student learning web development with Code the Dream.</p>
    </section>
    
    <section id="experience">
      <h2>Experience</h2>
      <ul>
        <li>JavaScript fundamentals</li>
        <li>Array methods and functions</li>
        <li>HTML structure</li>
      </ul>
    </section>
    
    <section id="connect">
      <h2>Connect</h2>
      <a href="https://github.com/johndoe">GitHub</a>
      <a href="https://linkedin.com/in/johndoe">LinkedIn</a>
    </section>
  </body>
</html>
```

## Variations That Are Acceptable

* **Different meta tags:** Students may include viewport, description, keywords, author, or other valid meta tags
* **More content:** Students may include more than the minimum required (more list items, more links, images, etc.)
* **Link organization:** Students may wrap links in `<ul>` and `<li>` tags (this is actually good practice!)
* **Additional elements:** Stretch goals like images, navigation, or footers are great additions
* **Formatting differences:** Extra line breaks or indentation styles don't affect functionality

## Red Flags (Request Revisions)

* **Copied boilerplate:** If they used a template generator instead of writing from scratch (first assignment should build muscle memory)
* **Missing required sections:** All three sections (About, Experience, Connect) must be present
* **No semantic HTML:** Should use `<section>`, not just `<div>` tags everywhere
* **Broken links:** Links should go to actual URLs (even if they're placeholder profiles)
* **JavaScript in HTML:** This is an HTML-only assignment; any JavaScript should be removed

## Feedback Tips

**Encourage:**
* "Great job writing your boilerplate from scratch!"
* "Your sections are well-organized and easy to read"
* "Nice use of semantic HTML with those section elements"

**Suggest improvements:**
* "Try adding a meta description to help with SEO"
* "Consider organizing your links in a list for better structure"
* "The viewport meta tag will help your site work better on mobile devices"

**For corrections:**
* "I notice you're missing a closing `</section>` tag on line X"
* "Your `<meta>` tags should be self-closing with `/>` at the end"
* "Make sure all your visible content is inside the `<body>` tags"
