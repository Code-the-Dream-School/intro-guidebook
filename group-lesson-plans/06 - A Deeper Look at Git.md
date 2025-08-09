# Week 6: A Deeper Look at Git — Group Mentor Guide

Welcome to Week 6 of the Intro to Programming course! This week, students are:

- Practicing Git commands in an interactive, visual context (via a game)  
- Building familiarity with branching, merging, and collaborative Git workflows  
- Visualizing how repositories can be duplicated, altered, and shared  
- *(Optional)* Continuing the stretch goal on algorithms to improve problem-solving strategies

Instead of a coding assignment, students are exploring Git concepts through **Oh My Git!** or **Learn Git Branching**.

## 🧊 Warm-Up (5–10 minutes)

Choose one:

**👋 Relationship-Building**  
- What’s a game or puzzle you’ve enjoyed that helped you learn something?  
- Share a time you successfully solved a problem by visualizing it differently.  

**💡 Check for Understanding (from last week)**  
- What does `git checkout -b branch-name` do?  
- When might you merge a branch into `main`?  
- What’s the difference between `git merge` and `git pull`?

## 🧭 Explore vs. Apply — Session Formats

**Explore Sessions** → Discuss branching and merging concepts, and demo these in a small repo. Show how they relate to collaborative workflows.
**Apply Sessions** → Have students share screens while playing *Oh My Git!* or *Learn Git Branching*. Work through specific branching/merging challenges together.

## ⏱️ Sample Timing for 1-Hour Session

| Time      | Activity                                               |
|-----------|--------------------------------------------------------|
| 0:00–0:10 | Warm-up + review Git basics from last week             |
| 0:10–0:25 | Explore: demo branching, merging, and resolving merges |
| 0:25–0:50 | Apply: game play, troubleshooting, group challenges    |
| 0:50–1:00 | Wrap-up + reflections                                  |

## ❓ Check for Understanding (Ask 2–3)

- Why use a branch instead of committing directly to `main`?  
- What does a “merge conflict” mean, and how do you resolve it?  
- How can branching help multiple people work on the same code base without overwriting each other’s work?  
- What’s the difference between a fast-forward merge and a regular merge?

## 🧑‍🏫 Explore Prompts

Demonstrate with a simple repo:

\`\`\`bash
# Create a new repo and branch
git init deeper-look
cd deeper-look
echo "Main file" > main.txt
git add main.txt
git commit -m "Initial commit on main"

# Create and switch to a feature branch
git checkout -b feature-branch
echo "Feature work" > feature.txt
git add feature.txt
git commit -m "Add feature file"

# Switch back to main and merge
git checkout main
git merge feature-branch
\`\`\`

Discuss:  
- What happens when branches have no conflicts?  
- How to handle conflicts if both branches modify the same line.  
- When to delete branches after merging.

## 🛠️ Apply Prompts (Live Troubleshooting & Gameplay)

### 🔧 Common Sticking Points
* Forgetting to commit before switching branches.  
* Confusion about local vs. remote branches.  
* Merge conflicts — not knowing how to edit and finalize the merge.  
* Not understanding what `HEAD` refers to in Git diagrams.  

### ✅ Try This Live
**Scenario:** A student tries to merge two branches and gets a conflict. Walk them through:  
1. Viewing the conflict in the file.  
2. Editing to keep the desired changes.  
3. Marking the conflict resolved with `git add`.  
4. Completing the merge with `git commit`.

## 💬 Engagement Strategies (for quiet groups)

- **Branch Challenge:** In pairs, create two branches that each make a change to the same file, then intentionally cause and resolve a merge conflict.  
- **Visual Guessing Game:** Show a Git graph and ask what commands were run to get there.  
- **Game Race:** Who can complete the first three levels of *Learn Git Branching* the fastest?

## 💡 Optional Challenges

- Complete all beginner levels in *Learn Git Branching*.  
- In *Oh My Git!*, complete one challenge involving a merge conflict.  
- Create a repo, make two branches, and merge them both into main — one clean merge, one with conflicts

✅ **Mentor To-Do**  
- [ ] Run a session using this guide.  
- [ ] Use visual or game-based exercises to reinforce Git branching/merging concepts.  
- [ ] Submit your [Mentor Session Report Form](https://airtable.com/appoSRJMlXH9KvE6w/shrp0jjRtoMyTXRzh).
