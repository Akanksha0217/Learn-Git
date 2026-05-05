# Git Cherry-Pick

## 📌 What is Git Cherry-Pick?

`git cherry-pick` is used to copy a specific commit from one branch and apply it to another branch.

Instead of merging the whole branch, you can pick only the commit you need.

---

## 🚀 Why use Cherry-Pick?

- Copy only one important commit
- Move bug fixes between branches
- Avoid merging unwanted changes

---

## 🧠 Syntax

```bash
git cherry-pick <commit-hash>
```

---

## 🔥 Example

### Branches:
- feature-login
- main

Suppose you fixed a bug in `feature-login` and want that same fix in `main`.

### Step 1: Find commit hash
```bash
git log
```

Example commit:
```bash
abc1234
```

---

### Step 2: Switch branch
```bash
git checkout main
```

---

### Step 3: Cherry-pick commit
```bash
git cherry-pick abc1234
```

👉 Now that specific commit is copied into `main`

---

## 📌 Cherry-pick multiple commits

```bash
git cherry-pick commit1 commit2 commit3
```

---

## 📌 Cherry-pick range of commits

```bash
git cherry-pick commit1^..commit3
```

👉 Picks all commits from commit1 to commit3

---

## ⚠️ If conflict happens

Git may show conflict while cherry-picking.

Resolve conflict, then run:

```bash
git add .
git cherry-pick --continue
```

---

## ❌ Cancel cherry-pick

```bash
git cherry-pick --abort
```

---

## 🔥 Real Use Case

Situation:
- You made 5 commits in feature branch
- Only 1 bug fix is needed in production

Instead of merging whole branch:

```bash
git cherry-pick bugfix_commit_hash
```

✅ Clean and efficient

---

## 🎯 Difference: Merge vs Cherry-Pick

| Feature | Merge | Cherry-pick |
|---|---|---|
| Copies all commits | ✅ Yes | ❌ No |
| Copies selected commit | ❌ No | ✅ Yes |
| Keeps branch history | ✅ Yes | Partial |

---

