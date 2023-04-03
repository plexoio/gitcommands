# Git Bash Commands Cheat Sheet

This is a cheat sheet of 100 commonly used commands in Git Bash, organized from basic to advanced, and from most used to least used. Each command includes a short explanatory comment.

## Concept

- [What is Git, Bash and Git Bash?](https://github.com/plexoio/gitcommands/blob/main/understanding-Git-and-Bash.md)

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
10. `git diff` # Show changes between working directory and the last commit
11. `git diff <branch1> <branch2>` # Show changes between two branches
12. `git show <commit>` # Show changes made in a specific commit
13. `git ls-files` # List all files tracked by Git
14. `git blame <file>` # Show who changed what in a file
15. `git bisect` # Find the commit that introduced a bug
16. `git reflog` # Show a log of all local commits
17. `git cat-file -p <commit>` # Display the content of a commit object
18. `git rev-parse <ref>` # Get the SHA-1 hash of a reference
19. `git fsck` # Verify the integrity of the repository
20. `git gc` # Clean up unnecessary files and optimize the repository

## Remote Repositories

21. `git remote add origin <url>` # Connect local repo to remote
22. `git push -u origin <branch>` # Push changes to remote branch
23. `git pull` # Pull changes from remote repo
24. `git clone <url>` # Clone a remote repository
25. `git remote -v` # List remote connections
26. `git remote rm <remote>` # Remove a remote connection
27. `git fetch` # Fetch updates from remote repo without merging
28. `git remote show <remote>` # Show details about a remote repository
29. `git remote rename <old-name> <new-name>` # Rename a remote repository
30. `git push --tags` # Push all tags to remote repository
31. `git push --force` # Force-push changes to the remote repository
32. `git push origin --delete <branch>` # Delete a remote branch
33. `git pull --rebase` # Pull and rebase the current branch
34. `git fetch --all` # Fetch updates from all remote repositories
35. `git remote update` # Update remote-tracking branches

## Branching & Merging

36. `git branch` # List all branches
37. `git branch <branch>` # Create a new branch
38. `git checkout <branch>` # Switch to a branch
39. `git checkout -b <branch>` # Create and switch to a new branch
40. `git merge <branch>` # Merge a branch into the current branch
41. `git branch -d <branch>` # Delete a branch
42. `git branch -r` # List remote branches
43. `git branch -a` # List local and remote branches
44. `git branch -u <upstream-branch>` # Set upstream branch for the current branch
45. `git branch -m <old-name> <new-name>` # Rename a branch
46. `git branch --merged` # List branches that have been merged into the current branch
47. `git branch --no-merged` # List branches that have not been merged into the current branch
48. `git merge --abort` # Abort an ongoing merge operation
49. `git merge --squash <branch>` # Squash the commits from a branch into a single commit
50. `git merge --no-ff <branch>` # Merge with a merge commit even if it's a fast-forward merge

## Stashing

51. `git stash` # Save changes for later
52. `git stash list` # List stashed changes
53. `git stash apply` # Apply stashed changes
54. `git stash drop` # Remove a stash
55. `git stash pop` # Apply and remove the latest stash
56. `git stash branch <branch>` # Create a new branch and apply a stash
57. `git stash save "<message>"` # Save changes with a custom stash message
58. `git stash clear` # Remove all stashed changes
59. `git stash apply <stash>` # Apply a specific stash
60. `git stash drop <stash>` # Remove a specific stash

## Rebase & Cherry-picking

61. `git fetch` # Fetch updates from remote repo
62. `git rebase <branch>` # Rebase current branch onto another
63. `git cherry-pick <commit>` # Apply a specific commit
64. `git rebase --abort` # Abort an ongoing rebase operation
65. `git rebase --continue` # Continue a paused rebase operation
66. `git rebase --skip` # Skip a conflicting commit during rebase
67. `git cherry-pick --continue` # Continue a paused cherry-pick operation
68. `git cherry-pick --abort` # Abort an ongoing cherry-pick operation

## Reset, Remove, and Rename

69. `git reset` # Reset staging area to match the last commit
70. `git reset <file>` # Remove a file from the staging area
71. `git reset --hard` # Discard all changes since the last commit
72. `git rm <file>` # Remove a file from the repository and working directory
73. `git mv <old-name> <new-name>` # Rename or move a file
74. `git clean -f` # Remove untracked files from the working directory
75. `git clean -fd` # Remove untracked files and directories from the working directory

## Tags

76. `git tag` # List tags
77. `git tag <tag-name>` # Create a lightweight tag
78. `git tag -a <tag-name> -m "<message>"` # Create an annotated tag
79. `git push origin <tag-name>` # Push a tag to the remote repository
80. `git tag -d <tag-name>` # Delete a local tag
81. `git push origin --delete <tag-name>` # Delete a remote tag
82. `git tag --contains <commit>` # Find tags containing a specific commit
83. `git describe` # Describe the most recent tag and commit

## Advanced Commands

84. `git submodule add <repository> <path>` # Add a Git submodule
85. `git submodule init` # Initialize Git submodules
86. `git submodule update` # Update Git submodules
87. `git submodule foreach <command>` # Execute a command in all submodules
88. `git grep <pattern>` # Search for a pattern in the repository
89. `git log -S"<pattern>"` # Search for commits that added or removed a pattern
90. `git archive --format=zip --output=<output-file> <branch>` # Create a zip archive of a branch
91. `git shortlog` # Summarize commit logs by author
92. `git log --graph --decorate --oneline` # Display commit history as a graph
93. `git rev-list --count <ref>` # Count the number of commits in a branch
94. `git commit --amend` # Modify the last commit
95. `git commit --amend -m "<new-message>"` # Modify the last commit message
96. `git reflog expire --expire=now --all` # Remove all reflog entries
97. `git rev-parse --show-toplevel` # Show the root directory of the repository
98. `git config --global alias.<alias-name> '<git-command>'` # Create a Git alias
99. `git config --list` # List all Git configuration settings
100. `git help <command>` # Show help for a Git command
