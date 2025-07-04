## General Commands

### 1. Commands

- git status (Shows the status of working directory and staging area (which files are changed, staged for commit, etc.))
- git log (Shows the commit history for the current branch.)
- git log --all --graph --decorate --oneline (Visualizes the commit history as a graph for all branches, with decorations and one-line summaries.)

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
