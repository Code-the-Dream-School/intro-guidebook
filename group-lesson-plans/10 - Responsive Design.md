### **Group Mentor Guide**

#### **Week 10: Responsive Design — Group Mentor Guide**
Welcome to Week 10! This week, students move from static layouts to **Responsive Design**. The goal is to ensure their portfolios look good on all devices, from mobile phones to large monitors. They will explore the **mobile-first approach**, **media queries**, and the **CSS Grid model**.

#### **Warm-Up (5–10 minutes)**
Choose one:
**Relationship-Building (Mindset: Willingness to Experiment)**
*   Think of something you failed at multiple times before you finally got it (a sport, a video game level, etc.). How did you keep yourself motivated to keep trying?
*   Have you witnessed someone else learn from a failure and then succeed? What strategies did they use?

**Check for Understanding (from CSS Layout)**
*   What is the difference between `justify-content` and `align-items` in Flexbox?
*   How do you link a navigation item to a specific section on the same page?

#### **Explore vs. Apply — Session Formats**
*   **Explore Sessions** → Demonstrate how media queries work by resizing the browser and show the difference between Flexbox and CSS Grid.
*   **Apply Sessions** → Help students implement their chosen approach (mobile-first vs. desktop-first) and troubleshoot media query breakpoints.

#### **Sample Timing for 1-Hour Session**
| Time | Activity |
| ------ | ------ |
| 0:00–0:10 | Warm-up + Review Git workflow (merging `lesson-9`) |
| 0:10–0:30 | Explore: Media Queries, relative units (%, REM, EM), and Grid basics |
| 0:30–0:50 | Apply: Live coding a media query or converting a section to Grid |
| 0:50–1:00 | Wrap-up: Discussion on "error messages as gifts" + Final questions |

#### **Check for Understanding (Ask 2–3)**
*   What is the "mobile-first" approach? (Answer: Coding the mobile layout as the default and adding media queries for larger screens).
*   Why is it better to use **percentages, REMs, or EMs** instead of pixels for sizing?.
*   What is the difference between a Flexbox layout and a **CSS Grid** layout?.
*   True or False: Error messages are a sign that you are a bad coder. (Answer: False—they are a "gift" and the key to learning).

#### **Explore Prompts**
*   **Media Query Live Demo:** Let's write a media query that changes the background color when the screen is wider than 768px.
*   **Relative Units:** Let's change a `font-size` from `px` to `rem`. What happens when we change the root font size?.
*   **Grid vs. Flexbox:** Let’s take the "Experience" section and try to build it using `display: grid` instead of flex. Which one feels more intuitive for this content?.

#### **Apply Prompts (Assignment Hotspots)**
*   **Git Branching:** Ensure students have merged `lesson-9` into `main` and pulled the changes before creating the `lesson-10` branch.
*   **Missing Media Queries:** Students must have at least **two** media queries defined.
*   **Specificity/Override Issues:** If a media query isn't working, check if the student's default CSS is placed *after* the media query (which might override it) or if the selector isn't specific enough.
*   **Complexity:** Remind students they only need to change a minimum of **two style properties** across **three elements** for each query.

#### **Optional Challenges**
*   **Stretch Goal:** Reformat the "Experience" or "Connect" sections to use a **Grid layout**.
*   **Mobile Testing:** Use the browser's "Inspect" tool to toggle device views and test their site on different phone models
