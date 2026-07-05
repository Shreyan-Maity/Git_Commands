
# 📘 Git Commands Guide 

A simple guide to understand Git commands in plain language.

---

## 🛠 Setup & Configuration
Before using Git, introduce yourself:

```bash
git --version                   # Check Git version
git config --global user.name   "Your Name"
git config --global user.email  "you@example.com"
git config --list               # Show all settings
```



## 📂 Starting a Project
```bash
git init                     # Start tracking a folder with Git
git clone <repo_url>         # Copy a project from GitHub
```



## 📋 Tracking Changes
```bash
git status                   # Show changed files
git add <file_name>          # Stage a file
git add .                    # Stage all files in current directory
git add -A                   # Stage all changes (new, modified, deleted) across repo
git diff                     # Show file differences
```



## 💾 Saving Work
```bash
git commit -m "message"      # Save snapshot with a message
git log                      # Show commit history
git show <commit-id>         # Show details of a commit
```



## 🌳 Branching & Merging
```bash
git branch                     # List branches
git branch <branch_name>       # Create new branch
git switch <branch_name>       # Switch branch (modern way)
git checkout -b <branch_name>  # Switch branch (older way, still works)
git merge <branch>             # Merge branch into current
```



## 🔄 Working with Remotes
```bash
git remote -v                  # Show linked repositories
git push origin <branch_name>  # Upload changes to GitHub
git pull origin <branch_name>  # Download changes from GitHub
git fetch                      # Get updates without merging
```



## 🧹 Undoing Mistakes
```bash
git restore <file>           # Undo changes in file
git reset <file>             # Unstage file
git reset --hard <commit-id> # Reset to commit (⚠️ deletes changes)
git revert <commit-id>       # Undo commit safely
```



## 📊 Collaboration Extras
```bash
git stash                    # Save changes temporarily
git tag <name>               # Mark commit (like version 1.0)
git blame <file>             # Show who changed each line
```



## 📝 Quick Reference Table

| Action              | Command Example            | Meaning                  |
|---------------------|----------------------------|--------------------------|
| Start project       | `git init`                 | Begin tracking folder    |
| Copy project        | `git clone URL`            | Download repo            |
| Check changes       | `git status`               | See modified files       |
| Stage file          | `git add file.txt`         | Select file to save      |
| Save snapshot       | `git commit -m "msg"`      | Save changes             |
| Switch branch       | `git switch branch-name`   | Move to another branch   |
| Upload to GitHub    | `git push origin main`     | Send changes online      |
| Download from GitHub| `git pull origin main`     | Get latest updates       |
| Undo file changes   | `git restore file.txt`     | Discard edits            |


✅ **Tip:** Start with `git init`, `git add`, `git commit`, and `git push/pull`. These are the core commands you’ll use daily. Once comfortable, explore branching and merging for team projects.

---

Here’s your **Git workflow guide**, showing both flows (`init → push` and `clone → push`) in a clean, copiable style:


# 🚀 Git Workflows

## 1️⃣ New Project: From Init to Push
```bash
# Step 1: Initialize Git in your project folder
git init

# Step 2: Check status of files
git status

# Step 3: Stage files (choose one)
git add <file_name>
git add .
git add -A

# Step 4: Commit changes with a message
git commit -m "Initial commit"

# Step 5: Link remote repository (GitHub, etc.)
git remote add origin <repo_url>

# Step 6: Push changes to remote (master/main branch)
git push -u origin <master/main>
```


## 2️⃣ Existing Project: From Clone to Push
```bash
# Step 1: Clone repository from remote
git clone <repo_url>

# Step 2: Move into project folder
cd <repo_name>

# Step 3: Check status of files
git status

# Step 4: Stage files (choose one)
git add <file_name>
git add .
git add -A

# Step 5: Commit changes with a message
git commit -m "Your commit message"

# Step 6: Push changes to remote (main branch)
git push origin <master/main>
```


## ⚡ Daily Shortcut Workflow
```bash
git status
git add -A
git commit -m "Update"
git push
```
