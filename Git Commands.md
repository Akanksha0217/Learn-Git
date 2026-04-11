# 🚀 Quick Setup

## 📌 Initialize Git
git init

## 📌 Add all files
git add .

## 📌 First commit
git commit -m "Initial commit"

## 📌 Connect to GitHub repository
git remote add origin https://github.com/your-username/your-repo-name.git

## 📌 Push code to GitHub
git branch -M main
git push -u origin main

# 🔄 Daily Workflow Commands

## 📌 Check status
git status

## 📌 Add changes
git add .

## 📌 Commit changes
git commit -m "Your message"

## 📌 Push to GitHub
git push

# 🌿 Branch Commands
## 📌 Create new branch
git checkout -b feature-branch

## 📌 Switch branch
git checkout main

## 📌 Merge branch
git merge feature-branch

# 🔁 Pull Latest Code
git pull origin main

# ❌ Undo Changes
## Undo last commit (keep changes)
git reset --soft HEAD~1

## Undo last commit (remove changes)
git reset --hard HEAD~1

# 🧹 Remove File from Git
git rm --cached filename

# 📦 Clone Repository
git clone https://github.com/your-username/your-repo-name.git
