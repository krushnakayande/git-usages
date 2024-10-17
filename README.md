# git-usages

Here’s a list of the most commonly used basic Git commands, along with a brief explanation for each:

### 1. **Git Configuration:**
   - Configure your user name and email, which is used for commits.

   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   ```

   To check the current Git configuration:
   ```bash
   git config --list
   ```

### 2. **Initializing a Repository:**
   - Create a new local Git repository.

   ```bash
   git init
   ```

### 3. **Cloning a Repository:**
   - Clone a remote repository to your local machine.

   ```bash
   git clone <repository-url>
   ```

### 4. **Checking Status:**
   - See the status of your working directory (which files are modified, staged, or untracked).

   ```bash
   git status
   ```

### 5. **Adding Files to Staging:**
   - Add changes to the staging area in preparation for a commit.

   Add specific files:
   ```bash
   git add <file>
   ```

   Add all modified files:
   ```bash
   git add .
   ```

### 6. **Committing Changes:**
   - Record changes to the repository with a descriptive message.

   ```bash
   git commit -m "Your commit message"
   ```

   To commit with a longer, multi-line message:
   ```bash
   git commit
   ```

### 7. **Viewing Commit History:**
   - Display the commit history of the project.

   ```bash
   git log
   ```

   For a compact history:
   ```bash
   git log --oneline
   ```

### 8. **Pushing to a Remote Repository:**
   - Push changes from your local repository to a remote repository.

   ```bash
   git push <remote> <branch>
   ```

   Example:
   ```bash
   git push origin main
   ```

### 9. **Pulling from a Remote Repository:**
   - Fetch and merge changes from a remote repository into your local branch.

   ```bash
   git pull
   ```

### 10. **Branching:**
   - Create a new branch.

   ```bash
   git branch <branch-name>
   ```

   - Switch to an existing branch.

   ```bash
   git checkout <branch-name>
   ```

   Or, create and switch to a new branch in one step:
   ```bash
   git checkout -b <branch-name>
   ```

### 11. **Merging Branches:**
   - Merge another branch into the current branch.

   ```bash
   git merge <branch-name>
   ```

### 12. **Deleting a Branch:**
   - Delete a local branch.

   ```bash
   git branch -d <branch-name>
   ```

   - Delete a remote branch:

   ```bash
   git push origin --delete <branch-name>
   ```

### 13. **Stashing Changes:**
   - Temporarily save changes that are not ready to be committed, so you can work on something else.

   ```bash
   git stash
   ```

   - To retrieve stashed changes:

   ```bash
   git stash pop
   ```

### 14. **Checking Differences:**
   - View changes that haven’t been staged yet:

   ```bash
   git diff
   ```

   - View differences between staged changes and the last commit:

   ```bash
   git diff --staged
   ```

### 15. **Resetting Changes:**
   - Unstage a file (but keep the changes).

   ```bash
   git reset <file>
   ```

   - Reset to the last commit (discard all changes):

   ```bash
   git reset --hard
   ```

### 16. **Removing Files:**
   - Remove a file from both the Git repository and the working directory:

   ```bash
   git rm <file>
   ```

   - Remove a file from the repository but keep it in the working directory:

   ```bash
   git rm --cached <file>
   ```

### 17. **Renaming Files:**
   - Rename a file and stage the change:

   ```bash
   git mv <old-name> <new-name>
   ```

### 18. **Tagging:**
   - Create a tag for a specific commit (commonly used for versioning):

   ```bash
   git tag <tag-name>
   ```

   - Push tags to a remote repository:

   ```bash
   git push origin --tags
   ```

### 19. **Fetching Changes:**
   - Download objects and refs from a remote repository but do not merge them.

   ```bash
   git fetch
   ```

### 20. **Undoing Commits:**
   - Undo the last commit (but keep the changes).

   ```bash
   git reset --soft HEAD~1
   ```

   - Undo the last commit (and discard the changes).

   ```bash
   git reset --hard HEAD~1
   ```

### 21. **Viewing Remote Repositories:**
   - List all remote repositories.

   ```bash
   git remote -v
   ```

   - Add a remote repository.

   ```bash
   git remote add <name> <url>
   ```

### 22. **Rebasing:**
   - Apply your branch’s commits on top of another base tip.

   ```bash
   git rebase <branch>
   ```

### 23. **Git Cherry-pick:**
   - Apply a specific commit from one branch to another.

   ```bash
   git cherry-pick <commit-hash>
   ```

### 24. **Git Revert:**
   - Undo a commit by creating a new commit that reverses the changes.

   ```bash
   git revert <commit-hash>
   ```

These are the basic commands that will get you started with Git. Let me know if you need help with any specific command or use case!
