# **GIT**

| Command                    | Description                                                       |
| -------------------------- | ----------------------------------------------------------------- |
| `git init`                 | Initialize a new Git repository in the current folder (locally)   |
| `git clone <url>`          | Copy (clone) a remote repository (use this instead of `git init`) |
| `git status`               | Show the status of changes (staged, unstaged, untracked)          |
| `git add *`                | Stage **all** modified and new files (not recommended)            |
| `git add <file>`           | Stage a specific **file** for the next commit |
| `git add ./<path>`         | Stage a specific **path** for the next commit |
| `git commit -m "message"`  | Save (commit) the staged changes with a message          |
| `git log`                  | View the history of commits                              |
| `git diff`                 | Show changes not yet staged or committed                 |
| `git branch`               | List all branches in the repo                            |
| `git branch <name>`        | Create a new branch                                      |
| `git checkout <branch>`    | Switch to a different branch                             |
| `git checkout -b <branch>` | Create and switch to a new branch in one command         |
| `git merge <branch>`       | Merge another branch into the current one                |
| `git pull`                 | Fetch and merge changes from the remote repository       |
| `git push`                 | Upload local commits to the remote repository            |
| `git remote -v`            | Show connected remote repositories                       |
| `git reset --hard HEAD`    | Discard all changes and return to the last commit        |
| `git rm <file>`            | Remove a file from the repo and stage the removal        |
| `git stash`                | Temporarily save changes you don’t want to commit yet    |
| `git stash pop`            | Re-apply the most recently stashed changes               |
