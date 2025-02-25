# Github_Commands.

### 1. **Cloning a repository**
Clone a repository to your local machine:
```bash
git clone <repository-url>
```

### 2. **Checking the status**
Check the status of the working directory (which files are modified, untracked, etc.):
```bash
git status
```

### 3. **Adding changes**
Add changes to the staging area before committing:
```bash
git add <file-name>      # Add a specific file
git add .                # Add all changes
```

### 4. **Committing changes**
Commit changes with a descriptive message:
```bash
git commit -m "Your commit message"
```

### 5. **Pushing changes**
Push committed changes to the remote repository on GitHub:
```bash
git push origin <branch-name>
```
For example:
```bash
git push origin main
```

### 6. **Pulling changes**
Pull the latest changes from the remote repository:
```bash
git pull origin <branch-name>
```
For example:
```bash
git pull origin main
```

### 7. **Creating a new branch**
Create a new branch and switch to it:
```bash
git checkout -b <new-branch-name>
```

### 8. **Switching branches**
Switch between existing branches:
```bash
git checkout <branch-name>
```

### 9. **Merging branches**
Merge changes from one branch into the current branch:
```bash
git merge <branch-name>
```

### 10. **Viewing commit history**
View the commit history:
```bash
git log
```

### 11. **Viewing remote repositories**
List all remote repositories associated with your project:
```bash
git remote -v
```
Sure! Here are more GitHub/Git commands that you can use in various scenarios:

### 12. **Removing a file**
Remove a file from the staging area and your working directory:
```bash
git rm <file-name>
```
If you just want to remove a file from staging but not delete it:
```bash
git rm --cached <file-name>
```

### 13. **Renaming a file**
Rename a file and stage it for commit:
```bash
git mv <old-filename> <new-filename>
```

### 14. **Viewing the difference (diff)**
See what has changed in your working directory (uncommitted changes):
```bash
git diff
```

See what has changed between commits or branches:
```bash
git diff <commit-id1> <commit-id2>
```

### 15. **Stashing changes**
If you need to temporarily save changes that you don’t want to commit yet, you can stash them:
```bash
git stash
```
To see stashed changes:
```bash
git stash list
```
To apply the latest stash:
```bash
git stash apply
```
To apply a specific stash:
```bash
git stash apply stash@{stash-number}
```

### 16. **Undoing a commit**
If you need to undo the last commit but keep your changes in the working directory:
```bash
git reset --soft HEAD~1
```
If you want to discard the last commit entirely (including changes):
```bash
git reset --hard HEAD~1
```

### 17. **Fetching changes**
Fetch the latest changes from the remote repository without merging them:
```bash
git fetch
```

### 18. **Tracking branches**
To create a local branch that tracks a remote branch:
```bash
git checkout --track origin/<branch-name>
```

### 19. **Deleting a branch**
To delete a local branch after it’s been merged:
```bash
git branch -d <branch-name>
```
Force delete a branch (even if it hasn't been merged):
```bash
git branch -D <branch-name>
```

To delete a remote branch:
```bash
git push origin --delete <branch-name>
```

### 20. **Renaming the current branch**
To rename the current branch:
```bash
git branch -m <new-branch-name>
```

### 21. **Rebasing**
To rebase your branch onto another branch (usually to avoid merge commits):
```bash
git rebase <branch-name>
```

To continue after a conflict during a rebase:
```bash
git rebase --continue
```

### 22. **Tagging**
Create a tag for a specific commit:
```bash
git tag <tag-name> <commit-id>
```
Push tags to the remote repository:
```bash
git push origin <tag-name>
```

Push all tags to the remote repository:
```bash
git push origin --tags
```

### 23. **Viewing a file's history**
View the history of a specific file:
```bash
git log <file-name>
```

### 24. **Reverting a commit**
If you want to undo a commit by creating a new one that undoes the changes:
```bash
git revert <commit-id>
```

### 25. **Interactive Rebase**
To interactively rebase commits (for example, to edit, squash, or reorder commits):
```bash
git rebase -i <commit-id>
```

### 26. **Squashing commits**
If you want to combine multiple commits into one, use interactive rebase:
```bash
git rebase -i HEAD~<number-of-commits>
```
Then, mark the commits to be squashed (s) and save. This will combine them into one commit.

### 27. **Checking Git configuration**
Check your Git configuration settings:
```bash
git config --list
```

### 28. **Changing the author of a commit**
To change the author information for the most recent commit:
```bash
git commit --amend --author="New Name <new.email@example.com>"
```

### 29. **Viewing remote branches**
To list all remote branches:
```bash
git branch -r
```

### 30. **Create and push a new tag**
To create a new tag:
```bash
git tag -a <tag-name> -m "Tagging version 1.0"
```
To push the tag to the remote:
```bash
git push origin <tag-name>
```

### 31. **Forking a repository (GitHub-specific)**
If you want to fork a repository on GitHub (usually done via GitHub's website interface), you click the "Fork" button. Once done, you can clone it to your local machine with:
```bash
git clone <forked-repository-url>
```

### 32. **Creating and opening a pull request**
GitHub does not have a direct Git command for pull requests. After pushing your branch to GitHub, you can create a pull request through the GitHub website.

---
