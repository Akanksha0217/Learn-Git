# Git Reset vs Revert

## 📌 Overview

Both `git reset` and `git revert` are used to undo changes in Git, but they work in completely different ways.

---

## 🔥 Key Difference

| Feature       | git reset 🧨               | git revert 🔒             |
|---------------|----------------------------|---------------------------|
| History       | Changes history            | Keeps history             |
| Safe for team | ❌ No                      | ✅ Yes                   |
| Use case      | Local changes              | Shared/public commits     |

---

## 🧠 git reset

### 📌 What it does:
Moves the HEAD pointer and removes commits.

---

### Types of reset:

#### 1. Soft Reset
```bash
git reset --soft HEAD~1
```
👉 Keeps changes in staging area

2. Mixed Reset (default)
```
git reset HEAD~1
```

👉 Keeps changes in working directory

3. Hard Reset 🚨
```
git reset --hard HEAD~1
```

👉 Deletes commit + changes permanently
🧠 git revert
📌 What it does:

Creates a new commit that undoes previous changes.
```
git revert HEAD
```
