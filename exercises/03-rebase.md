# Exercise 3 — Rebase a Feature Branch

## Goal
Replay a feature commit on top of a newer `main`.

Use a disposable repository/branch and start clean.

1. Create a feature branch:
   ```bash
   git switch main
   git switch -c feature-rebase-demo
   ```
2. Make a small change to `README.md`, then commit it:
   ```bash
   git add README.md
   git commit -m "Add feature notes"
   ```
3. Create a new commit on `main`:
   ```bash
   git switch main
   ```
   Edit `README.md`, then:
   ```bash
   git add README.md
   git commit -m "Update project documentation"
   ```
4. Rebase the feature branch:
   ```bash
   git switch feature-rebase-demo
   git rebase main
   ```
5. Inspect the graph:
   ```bash
   git log --oneline --graph --all
   ```

If a conflict occurs, resolve it, `git add` the resolved files, then run `git rebase --continue`. To abandon the rebase, use `git rebase --abort`.

Rebase rewrites the replayed commits. Avoid rebasing shared commits without coordinating with collaborators.
