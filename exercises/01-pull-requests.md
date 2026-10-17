# Exercise 1 — Feature Branch and Pull Request

## Goal
Create a feature branch, push it, and open a PR into `main`.

1. Update `index.html` on a feature branch:
   ```bash
   git switch -c feature-add-skills
   ```
2. Add a `Skills` section to the page.
3. Inspect and commit:
   ```bash
   git status
   git diff
   git add index.html
   git commit -m "Add skills section"
   ```
4. Push:
   ```bash
   git push -u origin feature-add-skills
   ```
5. On GitHub, open a PR with base `main` and compare `feature-add-skills`.
6. Inspect **Files changed** and write a clear PR description.
7. Make another commit on the same branch and push. Verify the existing PR updates.

## Review practice
Ask a collaborator to leave a comment or request a change. Fix it on the same branch, commit, and push again. A separate account/collaborator is needed to demonstrate a real second-person review.
