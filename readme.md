## General Commands

### 1. Commands

- git status (Shows the status of working directory and staging area (which files are changed, staged for commit, etc.))
- git log (Shows the commit history for the current branch.)
- git log --all --graph --decorate --oneline (Visualizes the commit history as a graph for all branches, with decorations and one-line summaries.)
- git push origin --force-with-lease (This pushes only if the remote hasn't changed since your last fetch.It protects you from accidentally overwriting someone else's new commits.)

## Commit in Git

### 1. Commit All Tracked, Modified Files

git commit -am "Your commit message"

- `git commit -a` automatically stages **all tracked, modified files** (but **not** new untracked files) and then commits them.
- The `-m` flag lets you specify the commit message directly in the command.

### 2. Commit All Changes Including New (Untracked) Files

git add . && git commit -m "Your commit message"

- `git add .` stages **all changes**, including new files.
- `git commit -m "Your commit message"` commits everything that was staged.

### Branches

- git branch (Lists all local branches)
- git branch -a (Lists all local and remote branches)
- git checkout branch-name (Switches to the specified branch)
- git checkout -b branch-name (Create and switches to the specified branch)

### Never do

- Don't rebase main branch and rebase rewrite the history of branch, it may risk and add some issue. So stay stick with git merge always in case of main branch.
- You don't generally "pull" changes into main via rebase — instead, you merge or fast-forward main with a branch:
- git checkout feature1 > git rebase main
- git checkout main > git merge feature1 (Don't do rebase)
