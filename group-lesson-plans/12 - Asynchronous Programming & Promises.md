#### **Lesson 12: Asynchronous Programming & DOM Forms — Group Mentor Guide**
Welcome to Lesson 12! This week is a hybrid of theory and practice. Students will explore the concepts of **Asynchronous Programming and Promises** while completing a hands-on assignment to build a functional **Message Form** using DOM manipulation.

#### **Warm-Up (5–10 minutes)**
Choose one:
**Relationship-Building (Mindset: Information Literacy/AI)**
*   Share a time you received bad advice or misinformation (perhaps from an AI tool). How did you realize it was wrong?
*   As a developer, what "clues" do you use to decide if a tutorial or documentation is trustworthy and applicable to your specific version of a tool?

**Check for Understanding (Asynchronous Theory)**
*   What is the main difference between **synchronous** and **asynchronous** code? (Answer: Synchronous runs one instruction at a time in order; asynchronous allows multiple tasks to run simultaneously in the background).
*   What are the three possible states of a **Promise**? (Answer: Pending, Fulfilled, and Rejected).

#### **Explore vs. Apply — Session Formats**
*   **Explore Sessions** → Walk through the "chameleon" nature of Promises and how `.then()` and `.catch()` act as a safety net for async results.
*   **Apply Sessions** → Live-code the **Message Form** logic, focusing on event listeners and DOM traversal to remove items.

#### **Sample Timing for 1-Hour Session**
| Time | Activity |
| ------ | ------ |
| 0:00–0:10 | Warm-up + Reviewing "Information Literacy" mindset |
| 0:10–0:25 | Explore: Async code and the `setTimeout` example |
| 0:25–0:50 | Apply: Handling form submission and creating list items dynamically |
| 0:50–1:00 | Wrap-up: Discussion on `preventDefault()` and `reset()` |

#### **Check for Understanding (Ask 2–3)**
*   Why is asynchronous code called "**non-blocking**"?
*   What does the `preventDefault()` method do during a form submission? (Answer: It stops the browser from automatically refreshing the page).
*   How do we access the value of a form field inside a "submit" event listener?
*   In DOM traversal, how can you find the parent of a button that was just clicked? (Answer: The `parentNode` property).

#### **Apply Prompts (Assignment Hotspots)**
*   **Git Workflow:** Remind students to merge their `lesson-11` PR and pull the changes to `main` before starting the `lesson-12` branch.
*   **The Mailto Link:** Ensure students use the `mailto:` prefix for the user's email link in the new list item.
*   **Removal Logic:** If students are stuck on the "remove" button, demonstrate how to use `event.target.parentNode.remove()`.
*   **Form Reset:** Remind students to call the `.reset()` method at the very end of the callback to clear the input fields
