#### **Lesson 9: CSS Layout**
| Week | Topic | Learning Objective |
| ------ | ------ | ------ |
| 9 | CSS Layout | Students will build layouts using Flexbox, implement internal site navigation, and understand the basics of web accessibility (A11y). |

#### **Assignment Rubric**
You can mark the student's assignment as complete if they:
* [ ] Successfully merged `lesson-8` and submitted `lesson-9` via a new pull request.
* [ ] Added a `<nav>` element with internal links to all sections.
* [ ] Created "Skills" and "Projects" sections with appropriate IDs.
* [ ] Used **Flexbox** to reformat the "Experience" and "Connect" sections.
* [ ] Included an empty `<ul>` in the Projects section for future use.

#### **Required Deliverables Checklist**
* **HTML Structure:**
    * [ ] `<nav>` element contains links to "About", "Experience", "Skills", "Projects", and "Connect".
    * [ ] "Skills" section exists with an `h2` and an `id`.
    * [ ] "Projects" section exists with an `h2`, an `id`, and an empty `<ul>`.
* **CSS/Flexbox:**
    * [ ] "Experience" section uses Flexbox (ideally showing job titles/dates in a row/column format).
    * [ ] "Connect" section uses Flexbox to align social media links or icons.
* **Git/Workflow:**
    * [ ] Assignment submitted via a GitHub Pull Request URL.

#### **What to Look For**
* **Internal Link Functionality:** Click the nav links; they should "jump" the page to the corresponding section.
* **Flexbox Implementation:** Check `index.css` to ensure they applied `display: flex` to the parent containers of the items they wanted to align.
* **Accessibility (Mindset):** While not a hard coding requirement, check if they used semantic elements like `<nav>` and `<section>` as discussed in the mindset and previous lessons.

#### **Sample CSS Snippets (For Reference)**
*Flexbox for Experience Section:*
```css
.experience-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

*Sticky Header (Stretch Goal):*
```css
header {
  position: sticky;
  top: 0;
}
```
