### **Resource 1: Group Mentor Guide**

#### **Week 9: CSS Layout — Group Mentor Guide**
Welcome to Week 9! This week, students shift from basic styling to **layout and positioning**, specifically focusing on **Flexbox** to organize content. They are also learning about **web accessibility (A11y)** and how to implement **internal navigation**.

#### **Warm-Up (5–10 minutes)**
Choose one:
**Relationship-Building**
* What is a website where you find it really easy to find what you're looking for? What about the layout makes it easy?
* Thinking about this week's mindset topic: Have you ever used a website that felt "broken" or difficult to navigate? How did that affect your experience?

**Check for Understanding (from CSS Basics)**
* What is the difference between **margin** and **padding**?
* How do we use a **class** vs. an **ID** in CSS?

#### **Explore vs. Apply — Session Formats**
* **Explore Sessions** → Demonstrate Flexbox properties (justify-content, align-items) and how internal links (`#id`) work.
* **Apply Sessions** → Debug Flexbox layouts in the "Experience" section or help students set up their navigation bar.

#### **Sample Timing for 1-Hour Session**
| Time | Activity |
| ------ | ------ |
| 0:00–0:10 | Warm-up + Review Git workflow (merging Lesson 8) |
| 0:10–0:30 | Explore: Flexbox basics & Internal Navigation links |
| 0:30–0:50 | Apply: Live coding the "Experience" or "Connect" layout |
| 0:50–1:00 | Wrap-up: Accessibility discussion + Final questions |

#### **Check for Understanding (Ask 2–3)**
* What CSS property must be applied to a parent container to start using Flexbox? (Answer: `display: flex`)
* How do you make a link "jump" to a specific section on the same page?
* What is the difference between `justify-content` and `align-items`?
* Why is accessibility (A11y) important for developers to consider from the start?

#### **Explore Prompts**
* **Internal Links:** Let's create a `<nav>` and link it to an ID. What happens if the ID doesn't match the `href`?
* **Flexbox Playground:** Let's take three boxes and try to center them perfectly. Which properties do we need?
* **The "Experience" Layout:** How can we use Flexbox to put a job title on the left and a date on the right?

#### **Apply Prompts (Assignment Hotspots)**
* **Missing `display: flex`:** Students often try to use `justify-content` without defining the container as a flex box.
* **Broken Internal Links:** Forgetting the `#` symbol in the `href` attribute (e.g., `href="skills"` instead of `href="#skills"`).
* **ID Consistency:** Using a different name for the section ID than what is used in the navigation link.
* **Git Branching:** Forgetting to pull the merged `main` branch before starting the `lesson-9` branch.

#### **Optional Challenges**
* **Stretch Goal:** Make the navigation header "sticky" or "fixed" so it stays at the top while scrolling.
* **A11y Check:** Use a tool like **WAVE** or **totA11y** to check the portfolio for accessibility errors.
* **Flexbox Froggy:** If the group is ahead, practice Flexbox levels together
