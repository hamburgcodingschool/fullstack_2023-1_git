# Git Cheat Sheet

This cheat sheet is for using the git command line tools on MacOS.

## New Git Projects

**Create a new git project / initialize git:**
```
git init
```

**Clone an existing git project:**
```
git clone <git@address.of.your/project.git>
```

## Making Commits

**What's the status in this git project?**
```
git status
```
- Green means: it has been staged for commit (git knows this change).
- Red means: it has not been staged and would not be committed.

**See what changed:**
```
git diff
```

**Add a change to git for the next commit:**
- This command stages the changed file for the next commit.
```
git add <filename>
```
- Add all files that you have been working on:
```
git add .
```

**Remove a change from the stage:**
- This command will remove a change from the stage so it will not be committed
- The change will not be lost
```
git restore --staged <filename>
```

**Remove a change completely:**
- This command removes a change that is not staged (red)
- The change will be lost
- The file will have the same state as before you changed it
```
git restore <filename>
```

**Make a git commit:**
```
git commit
```
- This will open vim
- Write the commit message and close with `:x`.
- If you don't want to use vim, you can use the command:
```
git commit -m "Your commit message"
```
- good practice: choose a simple commit message that describes precisely what has been changed

**See the history of commits:**
```
git log
```

## Branches

**Show all branches:**
```
git branch
```

**Create a new branch:**
```
git checkout -b <branch name>
```
- The `-b` stands for "branch".
- short for these two:
```
git branch feature
git checkout feature
```

**Move into an existing branch:**
```
git checkout <branch name>
```

**Merge branch `feature` into branch `master`:**
- First, you need to be on branch `master`.
- Then you can merge `feature` into `master` like this:
```
git merge feature
```

**Delete branch `feature`:**
```
git branch -d feature
```
- You cannot delete a branch you are on.
- If you want to delete a branch, you need to be on a different branch.
- If the branch is not fully merged yet, you get an error message.
- To delete the branch anyway:
```
git branch -D feature
```

## Other

**Get help:**
```
git --help
```