# new-interns-help
Git is a version control system (VCS) that helps track code changes, collaborate with teams, and manage different features of a project. This guide covers Git's key features, commands, and best practices.

# Git Workflow & Best Practices

## 1. Introduction
Git is a **version control system (VCS)** that helps track code changes, collaborate with teams, and manage different features of a project. This guide covers Git's key features, commands, and best practices.

---

## 2. Setting Up Git
### Install Git:
- **Windows:** Download from [git-scm.com](https://git-scm.com/) and install.
- **Mac:**
  ```sh
  brew install git
  ```
- **Linux:**
  ```sh
  sudo apt install git  # Debian-based
  sudo yum install git  # RHEL-based
  ```

### Configure Git (Run Once Per Machine)
```sh
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Check configuration:
```sh
git config --list
```

---

## 3. Git Basics
### Initialize a New Repository:
```sh
git init  # Creates a new Git repository in the current folder
```

### Clone an Existing Repository:
```sh
git clone <repo_url>  # Copies the repo to your local machine
```

### Check the Status of the Repository:
```sh
git status  # Shows modified, staged, and untracked files
```

---

## 4. Branching & Feature Branch Workflow
### Create & Switch to a New Branch:
```sh
git checkout -b feature-branch  # Creates and switches to a new branch
```

### View All Branches:
```sh
git branch  # Lists all branches
```

### Switch Branch:
```sh
git checkout main  # Switch back to main branch
```

### Delete a Branch:
```sh
git branch -d feature-branch  # Deletes a local branch
```

To delete a remote branch:
```sh
git push origin --delete feature-branch
```

---

## 5. Staging, Committing & Pushing Changes
### Stage Files:
```sh
git add .  # Adds all modified files to the staging area
```

### Commit Changes:
```sh
git commit -m "Descriptive commit message"
```

### Push Changes to Remote Repository:
```sh
git push origin feature-branch  # Pushes branch to GitHub
```

### Pull Latest Changes Before Pushing:
```sh
git pull origin main  # Updates local branch with remote changes
```

---

## 6. Merging & Resolving Conflicts
### Merge a Feature Branch into Main:
```sh
git checkout main  # Switch to main

git merge feature-branch  # Merge changes
```

### Handling Merge Conflicts:
1. Open the conflicting file(s).
2. Resolve conflicts manually.
3. Stage resolved files:
   ```sh
   git add conflicted-file.py
   ```
4. Commit the merge resolution:
   ```sh
   git commit -m "Resolved merge conflicts"
   ```

---

## 7. Undoing Changes & Reverting
### Undo the Last Commit (Keep Changes):
```sh
git reset --soft HEAD~1
```

### Undo the Last Commit (Discard Changes):
```sh
git reset --hard HEAD~1
```

### Unstage a File:
```sh
git reset HEAD file.py
```

### Revert a Specific Commit:
```sh
git revert <commit_hash>
```

---

## 8. Best Practices
✅ **Always create a new branch for features or bug fixes.**  
✅ **Write clear, descriptive commit messages.**  
✅ **Pull before pushing to avoid conflicts.**  
✅ **Use `.gitignore` to exclude unnecessary files.**  
✅ **Review and test code before merging to `main`.**  
✅ **Keep `main` branch stable and deployable.**  

---

## 9. Git Workflow Summary
| Action | Command | When to Do It |
|--------|---------|--------------|
| Initialize repo | `git init` | Start a new project |
| Clone repo | `git clone <repo_url>` | Get an existing repo |
| Check status | `git status` | Before committing changes |
| Stage files | `git add .` | Before committing changes |
| Commit changes | `git commit -m "message"` | After meaningful updates |
| Create a feature branch | `git checkout -b feature-name` | Before working on a new feature |
| Push to remote | `git push origin branch-name` | After committing changes |
| Pull latest changes | `git pull origin main` | Before pushing to avoid conflicts |
| Merge branches | `git merge feature-branch` | After feature is tested |
| Resolve conflicts | Edit files, `git add .`, `git commit` | If merge conflict happens |
| Delete old branches | `git branch -d feature-branch` | After merging |

---

## 10. Quick Git Cheat Sheet
```sh
git init  # Initialize Git repo
git clone <repo_url>  # Clone repo
git branch feature-name  # Create a new branch
git checkout feature-name  # Switch to branch
git add .  # Stage changes
git commit -m "commit message"  # Commit changes
git push origin feature-name  # Push branch to remote
git pull origin main  # Get latest updates
git merge feature-name  # Merge branch into main
git branch -d feature-name  # Delete the branch locally
git push origin --delete feature-name  # Delete the branch remotely
```

---

This guide should help you understand **how Git works, when to do what, and best practices to follow**. 🚀


