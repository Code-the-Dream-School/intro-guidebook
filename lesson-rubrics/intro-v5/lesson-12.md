#### **Lesson 12: Asynchronous Programming & Forms**
| Week | Topic | Learning Objective |
| ------ | ------ | ------ |
| 12 | Forms & Async | Students will implement a functional HTML form, manage DOM events, and understand the foundational concepts of Promises and non-blocking code. |

#### **Assignment Rubric**
You can mark the student's assignment as complete if they:
*   [ ] Merged `lesson-11` and submitted `lesson-12` via a new pull request.
*   [ ] **HTML:** Added a `<section>` with a form containing Name, Email, Message, and a Submit button.
*   [ ] **HTML:** Included a navigation link that jumps to the "Leave a Message" section.
*   [ ] **JS Submission:** Used `preventDefault()` to stop page refreshes and `reset()` to clear the form.
*   [ ] **JS Logic:** Successfully captured form values and appended them as a new `<li>` to the `#messages` section.
*   [ ] **JS Removal:** Each new message includes a "remove" button that deletes its specific list entry.
*   [ ] **Mindset:** Provided answers to the three prompts regarding Information Literacy and AI.

#### **What to Look For**
*   **Correct Selectors:** Check that `messageForm` is selected by its name attribute (`leave_message`) and the message list is queried within the `#messages` section.
*   **Dynamic HTML:** In `index.js`, the `newMessage` inner HTML should contain an `<a>` tag with a `mailto:` link and a `<span>` for the message.
*   **Event Delegation/Logic:** Ensure the "remove" button listener is defined *inside* the main form submission listener so it can be attached to each new list item as it's created.
*   **Styling:** Verify that the form and buttons have adequate spacing and appropriate sizing for mobile/touch interactions.

#### **Stretch Goals (Optional)**
*   [ ] Does the `#messages` section hide itself when the list is empty?
*   [ ] Did the student implement an "edit" button for message entries?
