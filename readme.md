# Git Command Cheat Sheet with Explanations

---

## ✅ Version & Configuration

```bash
# Check Git version
git --version

# View Git user configuration (global/local)
git config user.name
git config user.email

# Set Git user configuration globally
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

# Set Git user configuration for the current repository only
git config user.name "Your Name"
git config user.email "your@email.com"
```

---

## 📁 Basic File System Commands

```bash
# List files and folders in current directory
ls

# List all files including hidden ones (like .git)
ls -a

# Change directory to a specific folder
cd folder_name

# Go to the previous directory (parent folder)
cd ..

# Create a new file
touch filename.txt

# Create a new folder (directory)
mkdir folder_name
```

---

## 🔧 Git Initialization

```bash
# Initialize Git repository in the current directory
git init
```

---

## 📝 Editing Files in Terminal

```bash
# Open a file in nano editor
nano filename.txt

# Save file: Ctrl + O, then Enter
# Exit nano: Ctrl + X
```

---

## 🚥 Staging & Status

```bash
# View status of working directory
git status

# Stage a specific file
git add filename.txt

# Stage an entire folder
git add folder_name/

# Stage all changes (new, modified, deleted)
git add .
```

---

## 💾 Committing Changes

```bash
# Commit staged changes with a message
git commit -m "Your meaningful message"
```

---

## 📜 Viewing Commit History

```bash
# View full commit history
git log

# View detailed HEAD movement history
git reflog

# View condensed one-line history
git log --oneline
```

---

## ⏪ Undo/Reset

```bash
# Reset to a specific commit (DANGEROUS: deletes history!)
git reset --hard <commit-id>
```

---

## 🧹 Remove Files from Git

```bash
# Remove file from staging but keep it locally
git rm --cached filename.txt

# Remove file from both Git and local folder
git rm filename.txt
```

---

## 🚫 .gitignore

```bash
# Create a file named `.gitignore` and list files/folders to ignore:
node_modules/
.env
*.log
```

---

## 🌿 Branching

```bash
# List all local branches
git branch

# List all branches including remote
git branch -a

# Create a new branch
git branch new-branch

# Switch to another branch
git switch branch-name
# Or using older syntax:
git checkout branch-name

# Create and switch to a new branch
git switch -c new-branch
```

---

## 🔀 Merging

```bash
# Merge another branch into current branch
git merge other-branch

# If there is a conflict:
# - Open conflicted file
# - Manually fix the conflict
# - Stage and commit
```

---

## ✏️ Rename/Delete Branch

```bash
# Rename current branch
git branch -m new-name

# Delete a branch (safe)
git branch -d branch-name

# Delete a branch (force)
git branch -D branch-name
```

---

## 📦 Git Stash

```bash
# Save uncommitted changes
git stash

# Save all changes (including untracked)
git stash -a

# List stashes
git stash list

# Show latest stash diff
git stash show -p

# Apply and remove latest stash
git stash pop

# Apply stash but keep it
git stash apply

# Delete a specific stash
git stash drop stash@{0}

# Clear all stashes
git stash clear
```

---

## 🌐 Remote Repositories

```bash
# Clone a repository
git clone https://github.com/user/repo.git

# Add a remote repository
git remote add origin https://github.com/user/repo.git

# View remote URLs
git remote -v

# Push branch to remote
git push -u origin branch-name

# Pull latest changes from remote
git pull
```

---

## 🔍 Compare Changes

```bash
# See unstaged changes
git diff

# See staged changes
git diff --cached
```


