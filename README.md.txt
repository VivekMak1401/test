# Git Commands Guide

This document provides essential Git commands for managing repositories, collaborating on projects, and handling version control efficiently.

## **Setting Up Git**
### **Configure User Information**
Set up your Git username and email, which will be used in commit history.
```sh
git config user.name "Your Name"
git config user.email "your.email@example.com"
```
### **View Configured User Details**
Check your currently set username and email.
```sh
git config user.name
git config user.email
```

## **Initializing and Managing Repositories**
### **Initialize a Git Repository**
Create a new Git repository in the current directory.
```sh
git init
```
### **Check Repository Status**
Displays the state of the working directory and staging area.
```sh
git status
```

## **Working with Files**
### **Create and Navigate Directories**
Create a new directory and move into it.
```sh
mkdir project-name  # Create a new directory
cd project-name     # Navigate into directory
```
### **Create Files**
Create files in the working directory.
```sh
touch index.html  # Create an empty file
nano index.html   # Create and open file in editor
```

## **Staging and Committing Changes**
### **Add Files to Staging Area**
Prepare files for committing by adding them to the staging area.
```sh
git add index.html  # Add a specific file
git add .           # Add all files
```
### **Commit Changes**
Save changes permanently in the local repository.
```sh
git commit -m "Initial commit"
```

## **Viewing Commit History**
View the log of past commits.
```sh
git log             # View commit history
git log --oneline   # View concise history
```

## **Branching and Merging**
### **Create and Switch Branches**
Branches allow multiple versions of a project to be developed simultaneously.
```sh
git branch feature-1      # Create a branch
git checkout feature-1    # Switch to a branch
git checkout -b new-branch # Create and switch to a new branch
```
### **Merge Branches**
Integrate changes from one branch into another (e.g., merging a feature branch into main).
```sh
git checkout main
git merge feature-1
```
### **Delete a Branch**
Remove a branch that is no longer needed.
```sh
git branch -D feature-1
```

## **Undoing Changes**
### **Revert a Commit**
Create a new commit that undoes the changes from a previous commit.
```sh
git revert commit-id
```
### **Reset to a Previous Commit**
Move the branch pointer back to a previous commit, optionally discarding changes.
```sh
git reset commit-id  # Soft reset (keeps changes in working directory)
git reset commit-id --hard  # Hard reset (deletes changes)
```

## **Working with GitHub**
### **Connect Local Repo to GitHub**
Link a local Git repository to a remote repository on GitHub.
```sh
git remote add origin https://github.com/your-username/repo-name.git
git push -u origin main
```
### **Clone a Repository**
Download a remote Git repository to your local machine.
```sh
git clone https://github.com/user/repo.git
```

## **Collaboration and Pull Requests**
### **Fetch and Merge Latest Changes**
Retrieve updates from a remote repository and merge them into your local branch.
```sh
git pull origin main
```
### **Push Changes to GitHub**
Upload committed changes to a remote repository.
```sh
git push origin feature-branch
```
### **Create a Pull Request**
1. Push changes to GitHub.
2. Open GitHub and navigate to the repository.
3. Click on **"Compare & pull request"**.
4. Review changes and submit the pull request.

## **Forking and Contributing**
### **Fork a Repository and Clone Locally**
Create a copy of another repository in your account and clone it locally.
```sh
git clone https://github.com/your-username/forked-repo.git
```
### **Add Remote and Push Changes**
Sync your forked repo with the original repository and push changes.
```sh
git remote add upstream https://github.com/original-owner/repo.git
git push origin main
```
### **Create a Pull Request to the Original Repository**
- Go to GitHub.
- Navigate to **"Pull Requests"**.
- Open a new pull request for review.

---

This guide serves as a quick reference for essential Git and GitHub operations. 🚀
