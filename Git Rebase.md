# 🔄 Git Rebase & Advanced Concepts

---

## 📌 What is Git Rebase?

Rebase is used to **move or combine commits** from one branch to another.

👉 It creates a **clean, linear history** (no extra merge commits).

---

## 🔁 Rebase vs Merge

| Merge                | Rebase           |
| -------------------- | ---------------- |
| Keeps history        | Rewrites history |
| Creates merge commit | No extra commit  |
| Safe for teams       | Use carefully    |

---

## 🌿 Example Scenario

You have:

```id="1a2b3c"
main:     A---B---C
feature:       D---E
```

After rebase:

```id="4d5e6f"
main:     A---B---C---D'---E'
```

👉 D and E are reapplied on top of main

---

## ⚡ How to Use Rebase

Step 1: Switch to your branch

```bash id="gk83hs"
git checkout feature
```

Step 2: Rebase with main

```bash id="82hs7d"
git rebase main
```

---

## ⚠️ Rebase Conflict

If conflict happens:

```bash id="jsh82k"
git status
```

👉 Fix the file manually, then:

```bash id="ksh82j"
git add .
git rebase --continue
```

---

## ❌ Abort Rebase

```bash id="js82ks"
git rebase --abort
```

👉 Goes back to original state

---

## 🧹 Interactive Rebase (Advanced)

```bash id="ks82js"
git rebase -i HEAD~3
```

👉 You can:

* Edit commits
* Combine commits (squash)
* Delete commits

---

## 🍒 Cherry Pick

Used to copy **specific commit** from another branch

```bash id="82jshd"
git cherry-pick <commit-id>
```

---

## 🔍 View Commit History

```bash id="js82jd"
git log --oneline --graph
```

👉 Shows clean commit tree

---

## 🧠 When to Use Rebase?

✔ Clean project history
✔ Before merging your branch
✔ Personal branches

❌ Avoid on shared/public branches

---

## 💡 Best Practices

✔ Use rebase for cleaner commits
✔ Never rebase pushed code (team projects)
✔ Use interactive rebase for polishing commits

---

## 🎯 Summary

* Rebase = cleaner history
* Merge = safer option
* Cherry-pick = selective commit copy
* Use carefully in team projects

---

## 🚀 Next Topic Suggestion

👉 Git Hooks & Automation
