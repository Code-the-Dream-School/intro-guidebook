# Week 3: JavaScript Objects — Group Mentor Guide

Welcome to Week 3 of the Intro to Programming course! This week, students are learning:

- What objects are and how to write them
- The difference between primitives and objects
- Destructuring and accessing object data
- Working with dates, times, and built-in objects like `Math` and `Date`

Students are working in the `03-js-objects.js` assignment file.



## 🧊 Warm-Up (5–10 minutes)

Choose one:

**👋 Relationship-Building**  
- If your pet (real or imagined) had a superpower, what would it be?  
- What’s your favorite time of year, and why?

**💡 Check for Understanding (from last week)**  
- What’s the difference between an array and a string?  
- What happens if you forget to `return` something in a function?  
- What does `i++` mean again?



## 🧭 Explore vs. Apply — Session Formats

**Explore Sessions** → Walk through object structure, live-code `myPet`, break down template literals, or sketch out how dates work  
**Apply Sessions** → Debug student submissions, write new object examples, or remix object methods with the group



## ⏱️ Sample Timing for 1-Hour Session

| Time      | Activity                                |
|--|--|
| 0:00–0:10 | Warm-up + review last week              |
| 0:10–0:30 | Explore: build & explain object syntax  |
| 0:30–0:50 | Apply: live code + assignment help      |
| 0:50–1:00 | Wrap-up + final questions               |



## ❓ Check for Understanding (Ask 2–3)

- What’s the difference between a primitive and an object?
- What does `this` refer to inside an object method?
- How can we access a property in an object?
- What happens if we try to access a property that doesn’t exist?



## 🧑‍🏫 Explore Prompts

Use these to drive discussion and demystify objects:

- Let's build an object together. What kind of data could we store about your pet or a favorite movie?
- What are two ways to access properties in an object? When might each be useful?
- What’s the difference between `myObj.name` and `myObj["name"]`?

🧑‍💻 *Mini-Demo Ideas:*  

    // Object creation & access
    const myPet = {
      name: "Ziggy",
      species: "cat",
      color: "gray"
    };
    console.log(myPet.name);        // dot notation
    console.log(myPet["species"]);  // bracket notation

    // Object method using `this`
    const myPet = {
      name: "Ziggy",
      age: 3,
      getAge: function() {
        return this.age;
      }
    };
    console.log("Age:", myPet.getAge());



## 🛠️ Apply Prompts (Live Coding & Troubleshooting)

### 🔧 Assignment Hotspots
* Students forget to use `return` in object methods  
* `this` is misunderstood or replaced with variable name  
* Logging `undefined` due to typos in property names  
* Forgetting to call a method with `()` in `myPet.age()`  
* `Date` logic in Q5–Q7 can get tricky — walk through a sample  

### ✅ Try This Live

**Let’s walk through Q4 together — how can we check if an object is a dog?**

    function isDog(petObj) {
      let speciesChecker = "dog";
      return petObj.species === speciesChecker;
    }

Ask:
* How could we rewrite this to work with uppercase/lowercase mix?
* Can we refactor it into one line?



## 💬 Engagement Strategies (for quiet groups)

* Object Guessing Game: “I’ll describe an object — you tell me what the properties are.”  
* Group Remix: “Add a method to this object. What should it do?”  
* Time Travel Debug: “Here’s a `Date` bug — what’s going wrong?”



## 💡 Optional Challenges

- Write a new object called `myFavoriteBook` with at least one method.
- Stretch Goal from Q5: Convert month number to string using an array of month names.
- Rewrite Q10’s `reverseString` using `.split().reverse().join()`

    function reverseString(str) {
      return str.split("").reverse().join("");
    }



✅ Mentor To-Do  
- [ ] Run a session using this guide  
- [ ] Let students debug, explore, or build on their code  
- [ ] Submit your [Mentor Session Report](https://airtable.com/appoSRJMlXH9KvE6w/shrp0jjRtoMyTXRzh)
