# Exercise 2 — Merge Conflict

## Goal
Create and resolve a conflict on the same line.

Start from a clean working tree and a common `main` commit.

```bash
git switch main
git switch -c feature-heading-project
```

Change the `<h1>` in `index.html` to `Welcome to Our Project`, then commit:

```bash
git add index.html
git commit -m "Set project heading"
```

Create a second branch from the original `main`:

```bash
git switch main
git switch -c feature-heading-community
```

Change that same `<h1>` to `Welcome to Our Community`, then commit:

```bash
git add index.html
git commit -m "Set community heading"
```

Merge the second branch into the first:

```bash
git switch feature-heading-project
git merge feature-heading-community
```

Git should report a conflict. Open `index.html`, choose the final heading, and remove all conflict markers. Then:

```bash
git status
git add index.html
git commit -m "Resolve heading conflict"
```

Remember: during a merge, complete the merge with a commit. During a rebase, use `git rebase --continue` instead.
