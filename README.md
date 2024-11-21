# Version Control Git
This guide provides step-by-step instructions for handling essential Git and GitHub concepts with corresponding Git commands.

---

## **1. Creating a Repository**
### Steps:
1. On GitHub, click the `+` sign and select **New repository**.
2. Fill in the repository name, description, and visibility.
3. Check the box for **Add a README file** and click **Create repository**.
4. Open your terminal or Git Bash.
5. Navigate to the desired directory:

### Git Commands:
  ```bash
  cd /path/to/your/project
  ```
  ```bash
  # Initialize a new Git repository locally
  git init
  ```
  ```bash
  # Add a remote repository
  git remote add origin https://github.com/your-username/repository-name.git
  ```
---

## **2. Cloning a Repository**
### Steps:
1. Copy the repository URL from GitHub.
2. Open your terminal or Git Bash.
3. Navigate to the desired directory:
4. Clone the repository using:  
  ```bash
  git clone <repository_url>
  ```  
----

## 3. Creating Branches

### Steps:
1. Create a new branch:  
```bash
git branch <branch_name>
```
2. Switch to the new branch:
```bash
git checkout <branch_name>
```
3. Alternatively, create and switch to a branch in one step:
```bash
git checkout -b <branch_name>
```
---

## 4. Committing Changes
1. Stage the changes you made.
2. Commit the changes with a descriptive message.

### Steps:
  ```bash
  # Stage changes:
  git add .
  ```
  ```bash
  # Commit changes:
  git commit -m "Descriptive commit message"
  ```

---

## 5. Reverting Commits
1. Use git revert to undo specific commits.
2. This creates a new commit that undoes the changes from the reverted commit.

### Steps:
  ```bash
  # Revert the last commit:
  git revert HEAD
  ```
  ```bash
  # Revert a specific commit (use the commit hash):
  git revert <commit_hash>
  ```

---

## 6. Pulling and Pushing Changes
1. Pull to get the latest changes from the remote repository.
2. Push your changes to the remote repository.

```bash
# Pulling Changes (downstream)
git pull origin <branch_name>
```
```bash
# Pushing Changes (upstream)
git push origin <branch_name>
```

---

## 7. Fetching Changes
### Steps:
1. Fetch updates from the remote repository without merging them locally.

```bash
git fetch
```

---

## 8. Merging Branches
### Steps:
1. Switch to the branch you want to merge changes into.
2. Merge the target branch into the current branch.

```bash
# Switch to the branch you want to merge into:
git checkout <target_branch>
```
```bash
# Merge the other branch:
git merge <branch-name>
```
---

## 9. Renaming Branches
### Steps:
1. Rename the branch locally.
2. Push the renamed branch and delete the old branch remotely.
```bash
# Rename a branch locally
git branch -m old-branch-name new-branch-name
```
```bash
# Push the renamed branch
git push origin new-branch-name
```
```bash
# Delete the old branch remotely
git push origin --delete old-branch-name
```
---

## 10. Creating Pull Requests
### Steps:
1. Push your branch to the remote repository.
2. Go to GitHub and navigate to the repository.
3. Click Pull Requests > New Pull Request.
4. Select the source and target branches and click Create Pull Request.

---

## 11. Reviewing and Merging Pull Requests
### Steps:
1. Open the pull request on GitHub.
2. Review the changes and add comments if necessary.
3. Merge the pull request using the Merge Pull Request button.

---

## 12. Reverting Pull Requests
### Steps:
1. Go to the merged pull request on GitHub.
2. Click Revert to create a new commit that undoes the changes.
3. Review and merge the revert pull request.

```bash
# Revert a pull request by its commit hash
git revert commit-hash
```



   
   