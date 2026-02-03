# **Lesson 11 – The DOM API**

## **About This Week**
This week introduces students to the **Document Object Model (DOM)** and its role in creating interactive web pages. Students learn to identify how pages are structured, discover ways to **change the DOM**, and practice **traveling through the DOM (traversal)** to identify specific elements. By the end of the week, students should be able to dynamically add content to their pages using JavaScript, handle events, and use methods like `querySelector` and `createElement`.

## **Explore Session (60 minutes)**
**Purpose:** Reinforce understanding of how JavaScript interacts with HTML structure before students begin the assignment.
**Materials:** Mentor slides, code editor, and the lesson materials from The Odin Project or Scrimba.

### **Segment 1 – Warm-Up (5 min)**
*   **Ask:** “What do you think the browser does with your HTML before it displays it?”
*   **Quick poll:** “Can JavaScript change a CSS style without reloading the page?”

### **Segment 2 – I Do (10 min)**
**Mentor demonstrates DOM selection and modification:**
*   Explain **DOM Selection**: Show how to use `document.querySelector` or `getElementById` to find an element.
*   Explain **DOM Modification**: Show the difference between `innerHTML` and `textContent`.
*   **CFU Questions:** 
    *   “Why might we store a DOM element in a variable instead of selecting it every time?”
    *   “What happens to the existing content if we set a new `innerHTML` value?”

### **Segment 3 – We Do (20 min)**
**Collaborative example: Dynamically adding an element.**
*   Work together to create a new `paragraph` or `div` using `document.createElement`.
*   Set its content and use `appendChild` to add it to the body.
*   **CFU Questions:**
    *   “If we create an element in JS but don't append it, where does it live?”
    *   “How can we use a `for` loop to add multiple items to a list?”

### **Segment 4 – You Do (20 min)**
**Short Task:** 
*   “Create an array of three favorite foods. Use a loop to create an `<li>` for each and append them to an existing `<ul>` in your HTML.”
*   Share code snippets in the chat and discuss logic.

### **Segment 5 – Wrap-Up (5 min)**
*   Summarize: Selection → Creation → Modification → Appending.
*   **Remind:** Assignments are due **Feb 10, 2026**.

## **Apply Session (60 minutes)**
**Purpose:** Support students in completing the Lesson 11 assignment, focusing on the Skills section and Git workflow.

### **Segment 1 – Quick Recap (5 min)**
*   Address common Git issues: Ensure everyone has merged their `lesson-10` branch before starting `lesson-11`.

### **Segment 2 – Guided Coding (25 min)**
**Mentor demonstrates the Footer / Copyright task:**
*   Show how to use the `new Date()` constructor and `getFullYear()` to avoid hardcoding dates.
*   **CFU Questions:**
    *   “How do we find the relative path to our `index.js` file for the script tag?”
    *   “What is the difference between `append` and `appendChild`?”

### **Segment 3 – Peer or Solo Debugging (20 min)**
*   Troubleshoot the **Skills Section** loop.
*   Common bugs to look for: Forgetting to link the `<script>` tag before the closing `</body>` or incorrect ID names in `getElementById`.
