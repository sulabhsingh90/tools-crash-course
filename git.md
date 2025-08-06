# 🚀 Git Crash Course

> Your quick and practical guide to Git — the essential tool for version control.

*A one-liner guide for each command to help you get productive with Git fast.*

---

## 🔧 Setup

```bash
# Set your name and email globally
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global init.defaultBranch main  # Set default branch name to main
git config --list                            # View current config
```

---

## 📁 Initialize & Clone

```bash
# Start a new Git repository
git init
# Copy an existing repo locally
git clone <repo_url>
```

---

## 🔄 Staging & Committing

```bash
# Check current status of files
git status
# Stage a specific file
git add <file>
# Stage all files
git add .
# Commit staged files with message
git commit -m "Your message"
# Stage and commit in one step (only for tracked files)
git commit -am "Quick commit"
```

---

## 📤 Push & Pull

```bash
# Push local commits to remote
git push
# Pull latest commits and merge
git pull
# Fetch from remote (no merge)
git fetch
```

---

## 🌿 Branching

```bash
# List all branches
git branch
# Create a new branch
git branch <branch-name>
# Switch to a branch
git checkout <branch-name>
# Create and switch to a new branch
git checkout -b <branch-name>
# Merge branch into current branch
git merge <branch-name>
# Delete a branch
git branch -d <branch-name>
```

---

## 🧵 History & Logs

```bash
# View full commit history
git log
# View concise commit log
git log --oneline
# See unstaged changes
git diff
# See staged (added) changes
git diff --staged
# Show details of a commit
git show <commit-id>
```

---

## 🧹 Undo & Reset

```bash
# Undo changes in file (like Ctrl+Z)
git restore <file>
# Unstage a file
git reset <file>
# Discard all local changes ⚠️
git reset --hard
# Revert a commit by creating its opposite
git revert <commit-id>
```

---

## 🌐 Remote Repos

```bash
# View remote repo URLs
git remote -v
# Add a new remote repo
git remote add origin <url>
# Push and track upstream branch
git push -u origin main
```

---

## 🔍 Extras

```bash
# Save changes temporarily
git stash
# Reapply the last stashed changes
git stash pop
# Add a version tag
git tag <v1.0.0>
# Delete untracked files ⚠️
git clean -fd
```

---

## ✅ Pro Tips

* Always run `git status` before committing.
* Use `.gitignore` to exclude files from being tracked.
* For visuals:

  ```bash
  git log --graph --oneline --all
  ```

---

Happy committing! 🧫📂
