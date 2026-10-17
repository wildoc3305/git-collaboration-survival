# Exercise 5 — Recover with Reflog

## Safety
Use only a disposable practice repository/branch. `git reset --hard` can discard tracked working-tree and staging changes.

## Goal
Use reflog to locate a commit no longer at the branch tip.

1. Create a branch:
   ```bash
   git switch -c reflog-demo
   ```
2. Add a unique line to `README.md` and commit it:
   ```bash
   git add README.md
   git commit -m "Add recovery demo note"
   ```
3. Record the commit hash:
   ```bash
   git log -1 --oneline
   ```
4. Move the branch back one commit:
   ```bash
   git reset --hard HEAD~1
   ```
5. Inspect reference movements:
   ```bash
   git reflog
   ```
6. Copy the earlier commit hash from the reflog and inspect it:
   ```bash
   git show <commit-hash>
   ```
7. Create a recovery branch:
   ```bash
   git branch recovery-demo <commit-hash>
   git switch recovery-demo
   ```

The reflog is local and entries expire. It is a recovery aid, not a backup.
