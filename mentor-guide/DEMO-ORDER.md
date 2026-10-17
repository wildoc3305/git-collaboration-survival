# Mentor Demo Order

1. Show the GitHub repository, file list, branches, and commit history.
2. In the terminal run `git status`, `git branch`, and `git remote -v`.
3. Create a feature branch, edit `index.html`, commit, and push.
4. Open a PR; explain base vs compare and inspect **Files changed**.
5. Push a follow-up commit and show the existing PR update.
6. Use a second account/collaborator for a genuine review if available.
7. Demonstrate a merge conflict in the dedicated exercise.
8. Demonstrate rebase, cherry-pick, and reflog only in disposable practice branches.
9. Finish with `git log --oneline --graph --all`.

## Common diagnostics
```bash
git status
git branch -vv
git remote -v
git log --oneline --graph --all
git reflog
```

## Safety notes
- Never run `git reset --hard` on a repository with work you need.
- Rebase rewrites commit IDs; coordinate before rewriting shared history.
- Cherry-pick can conflict; resolve, stage, and use `git cherry-pick --continue`.
- During a rebase conflict, use `git rebase --continue`, not `git commit`.
- Keep a clean backup copy of the demo repository.
