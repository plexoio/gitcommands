# Git Bash Commands Cheat Sheet

This is a cheat sheet of the most commonly used commands in Git Bash, organized from basic to advanced, and from most used to least used. Each command includes a short explanatory comment.

## Updates

- This section will be updated over time.

## Basic Commands

1. `git init` # Initialize a new Git repository
2. `git config user.name "<name>"` # Set your Git username
3. `git config user.email "<email>"` # Set your Git email
4. `git status` # Check the status of your repo
5. `git add <file>` # Add a file to the staging area
6. `git add .` # Add all files to the staging area
7. `git commit -m "<message>"` # Commit changes with a message
8. `git log` # View commit history
9. `git log --oneline` # View commit history in compact format

## Remote Repositories

10. `git remote add origin <url>` # Connect local repo to remote
11. `git push -u origin <branch>` # Push changes to remote branch
12. `git pull` # Pull changes from remote repo
13. `git clone <url>` # Clone a remote repository

## Branching & Merging

14. `git branch` # List all branches
15. `git branch <branch>` # Create a new branch
16. `git checkout <branch>` # Switch to a branch
17. `git checkout -b <branch>` # Create and switch to a new branch
18. `git merge <branch>` # Merge a branch into the current branch
19. `git branch -d <branch>` # Delete a branch
20. `git push origin --delete <branch>` # Delete a remote branch

## Advanced Commands

21. `git stash` # Save changes for later
22. `git stash list` # List stashed changes
23. `git stash apply` # Apply stashed changes
24. `git stash drop` # Remove a stash
25. `git fetch` # Fetch updates from remote repo
26. `git rebase <branch>` # Rebase current branch onto another
27. `git cherry-pick <commit>` # Apply a specific commit
28. `git remote -v` # List remote connections
29. `git remote rm <remote>` # Remove a remote connection
30. `git diff` # Show changes between working directory and the last commit
31. `git diff <branch1> <branch2>` # Show changes between two branches
32. `git reset` # Reset staging area to match the last commit
33. `git reset <file>` # Remove a file from the staging area
34. `git reset --hard` # Discard all changes since the last commit
35. `git rm <file>` # Remove a file from the repository and working directory
36. `git mv <old-name> <new-name>` # Rename or move a file

## Git Aliases

37. `git config --global alias.<alias-name> '<git-command>'` # Create a Git alias
