# Week 5: Git Basics — Mentor Guide

Welcome to Week 5 of the Intro to Programming course! This week, students are learning:

- What a repository is and the benefits of version control systems like Git  
- How to create, clone, and organize a GitHub repository  
- How to stage, commit, and push changes to GitHub  
- How to create and submit a pull request for review  
- *(Optional)* Intro to algorithms as a stretch goal

Students are working on their **Git Basics** assignment, creating a repo, adding files, committing changes, and pushing to GitHub.

## Warm-Up (5–10 minutes)

Choose one:

**Relationship-Building**  
- What’s a “project” you’ve been proud to share with someone else?  
- What’s something new you’ve learned recently (inside or outside of tech)?  

**Check for Understanding (from last week)**  
- What’s the difference between the local files on your computer and files stored “in the cloud”?  
- Why might developers want to track the history of their code changes?  
- What’s an IDE and why might we use one?

## Explore vs. Apply — Session Formats

**Explore Sessions** → Walk through basic Git concepts (repo, commit, push) and demo creating & pushing a change to GitHub.  
**Apply Sessions** → Have students share screens to troubleshoot Git commands, fix common errors, or walk through pull request submissions.

## Sample Timing for 1-Hour Session

| Time      | Activity                                       |
|-----------|------------------------------------------------|
| 0:00–0:10 | Warm-up + review last week                     |
| 0:10–0:25 | Explore: demo repository creation & workflow   |
| 0:25–0:50 | Apply: students practice, troubleshoot issues  |
| 0:50–1:00 | Wrap-up + final questions                      |

## Check for Understanding (Ask 2–3)

- What is a Git repository, and how is it different from a regular folder?  
- What does `git add` do vs. `git commit`?  
- Why do we need to push commits to GitHub?  
- What’s the purpose of a pull request in our workflow?  
- What command would you use to create a new branch?

## Explore Prompts

Use these to demonstrate key concepts live:

1. **Creating a Repo** – Show creating a GitHub repo, initializing with a README, and cloning it locally.  
2. **Basic Workflow** – `git status` → `git add` → `git commit -m` → `git push origin branch-name`.  
3. **Branching** – `git checkout -b new-branch` and why branches are useful.  
4. **Pull Requests** – Walk through opening a PR and what happens after submission.

**Mini-Demo Ideas:**  

\`\`\`bash
# Create and move into new repo
git clone git@github.com:username/sample-repo.git
cd sample-repo

# Create and switch to a new branch
git checkout -b lesson-5

# Make a change
echo "Hello Git!" > index.html

# Stage and commit
git add index.html
git commit -m "Add index.html with greeting"

# Push to GitHub
git push origin lesson-5
\`\`\`

## 🛠️ Apply Prompts (Live Coding & Troubleshooting)

### 🔧 Assignment Hotspots
* Forgetting to create/switch to a branch before making changes.  
* Using `git add` but forgetting to commit before pushing.  
* Pushing to the wrong branch (or not specifying `origin branch-name`).  
* Confusing local changes vs. what’s on GitHub.  
* Not reading error messages carefully when push fails.  

### Try This Live

**Scenario:** A student has edited `README.md` but nothing is showing on GitHub. Ask:  
- What’s the output of `git status`?  
- Have they committed and pushed the changes?  
- Are they on the correct branch?  

## Engagement Strategies (for quiet groups)

- **Command Race:** “Type the Git command that stages all changes the fastest!”  
- **Error Sleuth:** Show a real Git error message and ask students how to fix it.  
- **PR Review Roleplay:** Have students explain the purpose of their pull request to a “reviewer.”

## Optional Challenges

- Clone a repo, create a branch, make a change, and open a PR — all without referring to notes.  
- Edit a file, commit with a meaningful message, then view the commit history with `git log`.  
- Make a small change to a file and undo it using Git commands.

✅ **Mentor To-Do**  
- [ ] Run a session using this guide.  
- [ ] Let students share screens to debug Git steps live.  
- [ ] Submit your [Mentor Session Report Form](https://airtable.com/appoSRJMlXH9KvE6w/shrp0jjRtoMyTXRzh).
