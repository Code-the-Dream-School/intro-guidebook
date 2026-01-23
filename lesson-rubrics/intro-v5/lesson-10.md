#### **Lesson 10: Responsive Design**
| Week | Topic | Learning Objective |
| ------ | ------ | ------ |
| 10 | Responsive Design | Students will apply basic design principles, implement media queries for mobile-first or desktop-first layouts, and experiment with CSS Grid. |

#### **Assignment Rubric**
You can mark the student's assignment as complete if they:
*   [ ] Successfully merged `lesson-9` and submitted `lesson-10` via a new pull request.
*   [ ] Defined at least **two media queries** in `index.css`.
*   [ ] Included comments to organize style sections (e.g., mobile, tablet, desktop).
*   [ ] Applied a minimum of **two style changes** to at least **three different elements** within *each* media query.
*   [ ] Used relative units (%, REM, or EM) for sizing elements.

#### **Required Deliverables Checklist**
*   **Media Queries:**
    *   [ ] Query 1 (e.g., Tablet): 3 elements changed, 2 properties each.
    *   [ ] Query 2 (e.g., Desktop): 3 elements changed, 2 properties each.
*   **Code Quality:**
    *   [ ] Comments used for organization.
    *   [ ] Use of relative units for responsiveness.
*   **Git/Workflow:**
    *   [ ] Assignment submitted via a GitHub Pull Request URL.

#### **What to Look For**
*   **Responsiveness:** Resize your browser window while viewing their site. Do the elements jump or resize as expected at the breakpoints?
*   **Unit Choice:** Check `index.css` to see if they are moving away from fixed `px` values towards more flexible units like `%`, `rem`, or `em`.
*   **Logic:** Did they follow a consistent approach (either mobile-first or desktop-first)?.
*   **Stretch Goal (Optional):** Check if they attempted to use `display: grid` for their "Experience" or "Connect" sections.

#### **Sample CSS Snippets (For Reference)**
*Example of a Mobile-First Media Query:*
```css
/* Tablet Styles */
@media (min-width: 768px) {
  h2 {
    font-size: 2rem; /* Change 1 */
    color: blue;    /* Change 2 */
  }
  .project-list {
    padding: 20px;  /* Change 1 */
    background: gray; /* Change 2 */
  }
  nav a {
    font-size: 1.2rem; /* Change 1 */
    font-weight: bold; /* Change 2 */
  }
}
```
