# Exercise 4 — Cherry-pick One Commit

## Goal
Apply one commit from another branch without merging the entire branch.

1. Create a source branch:
   ```bash
   git switch main
   git switch -c bugfix-demo
   ```
2. Add a clearly identifiable bug-fix note to `README.md`, then commit:
   ```bash
   git add README.md
   git commit -m "Fix navigation link"
   ```
3. Copy the commit hash:
   ```bash
   git log --oneline -1
   ```
4. Switch to the destination branch:
   ```bash
   git switch main
   ```
5. Apply the selected commit:
   ```bash
   git cherry-pick <commit-hash>
   ```
6. Inspect:
   ```bash
   git log --oneline --graph --all
   ```

If a conflict occurs, resolve it, stage the files, and run `git cherry-pick --continue`. To cancel the operation, run `git cherry-pick --abort`.
