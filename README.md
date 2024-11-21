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

### Steps:
1. Stage changes:
```bash
git add .
```
2. Commit changes with a message:
```bash
git commit -m "Your commit message"
```

---

## 5. Reverting Commits

### Steps:
1. Revert the last commit:
```bash
git revert HEAD
```
2. Revert a specific commit (use the commit hash):
```bash
git revert <commit_hash>
```

---

## 6. Pulling and Pushing Changes

### Pulling Changes
```bash
git pull origin <branch_name>
```
### Pushing Changes
```bash
git push origin <branch_name>
```

---

## 7. Fetching Changes
### Steps:
1. Fetch updates from the remote repository:
```bash
git fetch
```

---

## 8. Merging Branches
### Steps:
1. Switch to the branch you want to merge into:
```bash
git checkout <target_branch>
```
2. Merge the other branch:
```bash
git merge <source_branch>
```
---

## 9. Renaming Branches
### Steps:
1. Rename the current branch:
```bash
git branch -m <new-branch-name>
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



   
   