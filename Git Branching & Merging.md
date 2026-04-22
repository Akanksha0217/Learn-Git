# 🌿 Git Branching & Merging

## 📌 What is a Branch?

A branch in Git is like a **separate line of development**.

👉 It allows you to:

* Work on new features
* Fix bugs
* Experiment safely

Default branch = `main` (or `master`)

---

## 🌱 Creating a Branch

```bash
git branch feature-login
```

👉 This creates a new branch but does NOT switch to it.

---

## 🔀 Switching Branch

```bash
git checkout feature-login
```

OR (modern command):

```bash
git switch feature-login
```

---

## ⚡ Create + Switch (Shortcut)

```bash
git checkout -b feature-login
```

OR

```bash
git switch -c feature-login
```

---

## 📋 List All Branches

```bash
git branch
```

👉 Current branch will have `*`

---

## 🔁 Merging Branches

Step 1: Go to main branch

```bash
git checkout main
```

Step 2: Merge feature branch

```bash
git merge feature-login
```

---

## ⚠️ Merge Conflict

Happens when:
👉 Same file is changed in two branches

Git will show:

```
<<<<<<< HEAD
Your code
=======
Other branch code
>>>>>>> feature-login
```

👉 You must:

* Edit manually
* Remove conflict markers
* Then commit

---

## 🧹 Delete Branch

```bash
git branch -d feature-login
```

---

## 🌍 Remote Branch (GitHub)

Push branch to GitHub:

```bash
git push origin feature-login
```

---

## 🔥 Real Workflow Example

```bash
git checkout -b new-feature
# Do work
git add .
git commit -m "Added new feature"
git push origin new-feature
```

Then merge into main.

---

## 💡 Best Practices

✔ Use meaningful branch names
✔ Keep branches small
✔ Always pull latest code before merging
✔ Delete unused branches

---

## 🎯 Summary

* Branch = separate workspace
* Merge = combine changes
* Conflicts = manual fix
* Helps in teamwork

---

## 🚀 Next Topic Suggestion

👉 Git Rebase & Cherry-pick
