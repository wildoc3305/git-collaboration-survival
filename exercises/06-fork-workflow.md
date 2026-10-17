# Exercise 6 — Fork, Origin, Upstream

## Goal
Understand the fork-based contribution workflow.

1. Fork a repository you are allowed to contribute to on GitHub.
2. Clone your fork:
   ```bash
   git clone https://github.com/YOUR-USERNAME/REPOSITORY.git
   cd REPOSITORY
   ```
3. Inspect remotes:
   ```bash
   git remote -v
   ```
   `origin` normally points to your fork.
4. Add the original project as `upstream`:
   ```bash
   git remote add upstream https://github.com/ORIGINAL-OWNER/REPOSITORY.git
   ```
5. Fetch upstream:
   ```bash
   git fetch upstream
   ```
6. Create a feature branch, make a small change, commit, and push to your fork.
7. Open a PR from your fork's feature branch into the original repository's target branch.

Replace placeholder URLs with the real repository URLs. Forking does not grant write access to the original project.
