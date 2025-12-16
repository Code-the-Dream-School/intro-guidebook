# Week 5: Git Basics

## Assignment Overview
This week's assignment focuses on practicing the Git workflow rather than solving coding problems. Students are learning to create repositories, work with branches, make commits, and create pull requests—fundamental skills they'll use throughout the course.

## Review Checklist

Use this checklist when reviewing a student's Week 5 submission:

### Repository Setup
- [ ] Repository exists on student's GitHub account
- [ ] Repository name follows naming convention: `firstname-lastname-classname` (e.g., `maria-santiago-jupiter`)
- [ ] Repository has a description
- [ ] Repository is set to PUBLIC
- [ ] Repository was initialized with a README file

### Branch Structure
- [ ] Student created a branch called `lesson-5`
- [ ] Work was done on the `lesson-5` branch (not directly on `main`)
- [ ] Branch shows in GitHub branch list

### File Changes
- [ ] README.md file contains student's full name
- [ ] `index.html` file exists in the repository (at root level, same as README.md)
- [ ] Both files are present in the `lesson-5` branch

### Git Workflow
- [ ] Student made at least one commit with a message
- [ ] Commit message is descriptive (should be something like "my first commit" or better)
- [ ] Changes were pushed to GitHub successfully
- [ ] Student created a pull request from `lesson-5` to `main`

### Pull Request Quality
- [ ] Pull request title is clear
- [ ] PR shows the correct files changed (README.md and index.html)
- [ ] PR is from `lesson-5` branch into `main` branch

## Troubleshooting Tips for Mentors

### Student can't clone repository
**Likely causes:**
- SSH key not set up correctly
- Using HTTPS URL instead of SSH URL

**How to help:**
- Verify they completed "The Odin Project - Setting Up Git" lesson
- Have them try `ssh -T git@github.com` to test SSH connection
- Walk them through SSH key setup if needed

### Student's changes aren't showing on GitHub
**Likely causes:**
- Forgot to commit
- Forgot to push
- Pushed to wrong branch

**How to help:**
- Have them run `git status` and share output
- Have them run `git log` to see if commit exists
- Check if they ran `git push origin lesson-5` (not just `git push`)

### Student created files but they're not in the commit
**Likely causes:**
- Forgot to run `git add`
- Added wrong files

**How to help:**
- Have them run `git status` to see untracked files
- Walk them through `git add .` or `git add filename`
- Remind them to commit after adding

### Student accidentally worked on main branch
**How to help:**
- Don't worry—this is fixable!
- Option 1: Have them create `lesson-5` branch from current state: `git checkout -b lesson-5`
- Option 2: Have them reset main and redo on proper branch (more advanced, only if student is comfortable)
