⚡ Terminal & Git/GitHub Cheat Sheet

A concise reference for **Terminal commands**, **Git essentials**, and **GitHub workflows**.

---

📑 Table of Contents
- [💻 Terminal Basics](#-terminal-basics)
- [🌱 Git Fundamentals](#-git-fundamentals)
- [🔗 Git vs GitHub](#-git-vs-github)
- [🚀 Complete Workflow Example](#-complete-workflow-example)
- [💡 Pro Tips](#-pro-tips)

---

 💻 Terminal Basics

### Navigation & Files
| Command | Description |
|---------|-------------|
| `ls` | List files |
| `ls -la` | List all files (including hidden) with details |
| `pwd` | Show current directory path |
| `cd [dir]` | Change directory |
| `cd ..` | Move up one level |
| `mkdir [name]` | Create new directory |
| `touch file1 file2` | Create new files |
| `rm [file]` | Delete file |
| `rm -rf [dir]` | Force delete directory (⚠️ irreversible) |

### Shortcuts
- `Tab` → Auto-complete file/directory names
- `↑/↓` → Navigate command history
- `Ctrl+C` → Stop current process

---

 🌱 Git Fundamentals ⚙️ First-Time Setup

git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --global init.defaultBranch main

📂 Starting a Project

`git init`  # Initialize new repository

#🔄 Common Workflow

`git add .`                      # Stage changes
`git commit -m "message"`        # Commit
`git remote add origin repo_url`  # Connect to GitHub
`git push -u origin main `       # Push

📊 File Stages in Git

`Untracked` → Not in Git

`Staged` → Added with git add

`Committed` → Saved locally

`Pushed` → Uploaded to GitHub

🌿 Branching

`git branch `             # List branches
`git checkout branch`     # Switch branch
`git checkout -b new`     # Create + switch
`git branch -d branch`    # Delete branch
`git merge branch`        # Merge branch


♻️ Undoing Changes

##Unstage file

`git reset file_name`
`git reset`   # Unstage all


Undo last commit

`git reset HEAD~1`

Hard reset (⚠️ danger)

`git reset --hard commit_id`

🔗 Git vs GitHub

Git → Local version control system 🖥

GitHub → Cloud hosting platform ☁️

🚀 Complete Setup Example
# First time setup
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

# New project
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/username/repo.git
git push -u origin main

# Existing project
git clone https://github.com/username/repo.git
cd repo

💡 Tips

git commit -am "msg" → Add & commit tracked files in one step

git log --oneline → Compact history

git branch -m old new → Rename branch

git stash → Temporarily save changes

✨ These notes are designed as a quick reference for students & developers learning Git, GitHub, and terminal basics.

