# Git Collaboration Survival — Practice Repository

A hands-on practice project for GitHub collaboration, Pull Requests, merge conflicts, rebase, cherry-pick, and reflog.

## Prerequisites
- Git installed
- GitHub account
- VS Code or another editor
- A terminal

## Quick start
1. Create a **new empty GitHub repository** named `git-collaboration-survival`.
2. Download and extract this starter pack.
3. In the extracted folder, run:

```bash
git init
git branch -M main
git add .
git commit -m "Initial practice project"
git remote add origin https://github.com/YOUR-USERNAME/git-collaboration-survival.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your GitHub username. If you created a README on GitHub while creating the repository, create the repository empty instead to avoid unrelated history.

## Suggested practice order
1. `exercises/01-pull-requests.md`
2. `exercises/02-merge-conflicts.md`
3. `exercises/03-rebase.md`
4. `exercises/04-cherry-pick.md`
5. `exercises/05-reflog.md`
6. `exercises/06-fork-workflow.md`

## Safety
Perform `git reset --hard` exercises only in a disposable practice branch/repository. It can discard tracked working-tree and staging changes. Never use it on important uncommitted work.

## Project structure
- `index.html` — small website for feature-branch and PR exercises
- `style.css` — basic styling
- `exercises/` — step-by-step guided exercises
- `mentor-guide/` — demonstration notes and expected outcomes
