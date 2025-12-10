# Git Repository Management Lab

## Overview
This repository contains all work completed for the Git Repository Management Lab, where you learn to configure Git, create repositories, make commits, create branches, merge changes, and push code to GitHub.

---

## Lab Tasks and Commands

### Task 1: Configure Git (One-time Setup)
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --global --list
```
**Expected Output**  
You should see your username, email, and other default Git settings.

---

### Task 2: Initialize a Local Repository
```bash
mkdir git-lab
cd git-lab
git init
```
**Expected Output**  
Initialized empty Git repository in git-lab directory

---

### Task 3: Create Your First Commit
```bash
echo "Hello Git!" > readme.txt
git status
git add readme.txt
git commit -m "Initial commit: Added readme file"
```

---

### Task 4: Create and Work on a Branch
```bash
git branch feature-update
git checkout feature-update
echo "New feature added!" >> readme.txt
git add readme.txt
git commit -m "Updated readme with new feature text"
```

---

### Task 5: Merge the Branch Back to Main
```bash
git checkout main
git merge feature-update
```

---

### Task 6: Connect to GitHub
1. Create a new GitHub repo:  
   https://github.com/new

2. Add the GitHub remote:
```bash
git remote add origin https://github.com/<username>/git-lab.git
```

3. Push your project:
```bash
git push -u origin main
```

---

### Task 7: View Commit History
```bash
git reflog show --all
```

---

## Screenshots
- Git Config History — Script Execution  
- Git Init History — Script Execution  
- Commit History and Merge History — Script Execution

---
