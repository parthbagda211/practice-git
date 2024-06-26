Here are the steps to perform the requested Git operations:

1. **Set your username and email in Git config**:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your@email.com"
   ```

2. **Create a new branch named "feature-branch" and switch to it**:
   ```bash
   git checkout -b feature-branch
   ```

3. **List all branches in the repository**:
   ```bash
   git branch
   ```

4. **Delete the branch "feature-branch"**:
   ```bash
   git branch -d feature-branch
   ```

5. **Undo the last commit**:
   ```bash
   git reset HEAD~1
   ```

6. **Create a new branch named "conflict-branch"**:
   ```bash
   git checkout -b conflict-branch
   ```

7. **Create another branch named "feature1"**:
   ```bash
   git checkout -b feature1
   ```

8. **Make some changes in the "feature1" branch**:
   - Edit a file and make changes
   - `git add <file>`
   - `git commit -m "Changes in feature1"`

9. **Merge "feature1" branch into the main branch**:
   ```bash
   git checkout main
   git merge feature1
   ```

10. **Make changes in "conflict-branch", in the same file and line that you had made changes in "feature1"**:
    - Edit the conflicting file and make changes
    - `git add <file>`
    - `git commit -m "Changes in conflict-branch"`

11. **Merge the main branch into "conflict-branch"**:
    ```bash
    git checkout conflict-branch
    git merge main
    ```

12. **Resolve merge conflicts**:
    - Open the conflicting files and resolve the conflicts
    - `git add <resolved-files>`
    - `git commit -m "Resolve merge conflicts"`

13. **Add a remote named "origin" pointing to a GitHub repository**:
    ```bash
    git remote add origin https://github.com/username/repository.git
    ```

14. **Fork a repository on GitHub and clone it to your local machine**:
    ```bash
    git clone https://github.com/your-username/forked-repository.git
    ```

15. **Create a new branch on your fork, make changes, and open a pull request to the original repository**:
    ```bash
    git checkout -b new-feature
    # Make changes
    git add .
    git commit -m "Add new feature"
    git push origin new-feature
    ```
    - Open a pull request on GitHub from your fork to the original repository

16. **Comment on a PR and suggest improvements**:
    - Go to the pull request on GitHub
    - Add a comment with your suggestions

17. **Create a Git alias for the command `git log --oneline` named `gitlol`**:
    ```bash
    git config --global alias.gitlol "log --oneline"
    ```

18. **Create a pre-commit hook**:
    - Create a file named `pre-commit` in the `.git/hooks` directory
    - Add your hook script to the file
    - Make the file executable: `chmod +x .git/hooks/pre-commit`

19. **Switch to another branch without committing local changes**:
    ```bash
    git stash
    git checkout another-branch
    ```
    - When ready to return to the original branch: `git stash pop`

20. **Restore a deleted file using Git**:
    ```bash
    git checkout HEAD -- <file>
    ```

21. **Add a file to the last commit without creating a new commit**:
    ```bash
    git add <file>
    git commit --amend --no-edit
    ```

22. **Discard all changes in the working directory and revert to the last commit**:
    ```bash
    git checkout -- .
    ```

23. **View changes introduced by a specific commit**:
    ```bash
    git show <commit-hash>
    ```

24. **Change a commit message after committing**:
    ```bash
    git commit --amend -m "New commit message"
    ```

25. **Incorporate changes from a colleague's branch without merging**:
    ```bash
    git fetch origin colleague-branch
    git cherry-pick origin/colleague-branch
    ```

26. **Squash multiple commits into a single commit before pushing**:
    ```bash
    git rebase -i HEAD~n  # n is the number of commits to squash
    ```
    - In the interactive rebase editor, change "pick" to "squash" for the commits you want to squash
    - Save and exit the editor
    - Force push the changes: `git push --force-with-lease`

27. **Unstage a file**:
    ```bash
    git reset HEAD <file>
    ```

28. **Ignore files with .yml extension and files inside the config folder**:
    - Create a `.gitignore` file in the repository root
    - Add the following lines:
      ```
      *.yml
      config/
      ```

29. **List all files changed in the last commit**:
    ```bash
    git diff-tree --no-commit-id --name-only -r HEAD
    ```

30. **Fetch the latest changes from the remote repository without merging**:
    ```bash
    git fetch origin
    ```

31. **Recover a deleted branch**:
    ```bash
    git checkout -b recovered-branch origin/deleted-branch
    ```

32. **Remove untracked files and directories**:
    ```bash
    git clean -df
    ```

33. **Cherry-pick a commit from a feature branch to the main branch**:
    ```bash
    git checkout main
    git cherry-pick <commit-hash>
    ```

34. **Move a commit from one branch to another**:
    ```bash
    git checkout correct-branch
    git cherry-pick <commit-hash>
    ```

35. **Cherry-pick a range of commits from a feature branch**:
    ```bash
    git checkout main
    git cherry-pick <start-commit-hash>..<end-commit-hash>
    ```

36. **Clone a specific branch from a GitHub repository**:
    ```bash
    git clone -b branch-name https://github.com/username/repository.git
    ```

37. **Push local changes to a fork on GitHub**:
    ```bash
    git push origin main
    ```

38. **Create a new branch both locally and on GitHub**:
    ```bash
    git checkout -b new-feature
    git push -u origin new-feature
    ```

39. **View commit history of a GitHub repository**:
    ```bash
    git log
    ```

40. **Remove a sensitive commit from local and remote repositories**:
    ```bash
    git reset --hard HEAD~1
    git push origin +main
    ```

41. **Delete a remote branch on GitHub**:
    ```bash
    git push origin --delete remote-branch
    ```

42. **Create a Git repository for assignments, upload them, and request code reviews**:
    - Create a new repository on GitHub for your assignments
    - Clone the repository to your local machine
    - Add your assignments to the repository
    - Push the changes to GitHub
    - Share the repository with your peers and request code reviews
    - Review your peers' assignments

43. **Create a pull request on an open-source library on GitHub**:
    - Fork the open-source repository on GitHub
    - Clone your forked repository to your local machine
    - Create a new branch for your changes
    - Make your changes and commit them
    - Push your changes to your forked repository
    - Open a pull request from your forked repository to the original repository
    - Attach the pull request link to the README file of your project's repository
