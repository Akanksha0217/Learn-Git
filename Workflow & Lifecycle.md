# Git Workflow & Lifecycle

## 🔄 What is Git Workflow?

Git workflow defines how developers use Git to manage and track changes in a project.

---

## 📌 Basic Git Lifecycle

There are 3 main stages in Git:

1. Working Directory
2. Staging Area
3. Local Repository

---

## 🔁 Flow Diagram

Working Directory → Staging Area → Local Repository → Remote Repository

---

## 📌 Step-by-Step Workflow

### 🔹 1. Create or Clone Repository

```bash
git init
git clone <repo-url>
```

---

### 🔹 2. Make Changes

Edit or create files in your project.

---

### 🔹 3. Check Status

```bash
git status
```

---

### 🔹 4. Add Changes to Staging Area

```bash
git add .
```

---

### 🔹 5. Commit Changes

```bash
git commit -m "Added new feature"
```

---

### 🔹 6. Push to GitHub

```bash
git push origin main
```

---

### 🔹 7. Pull Latest Changes

```bash
git pull origin main
```

---

## 📌 Visual Understanding

* Working Directory → where you write code
* Staging Area → where you prepare changes
* Repository → where changes are saved permanently

---

## 📌 Common Workflow Example

1. git pull
2. make changes
3. git add .
4. git commit -m "message"
5. git push

---


## 🎯 Summary

Git workflow helps developers:

* Track changes efficiently
* Work collaboratively
* Maintain clean project history
