# Git and GitHub Basics

## Git Overview

Git is a free, open-source, scalable, superfast, and local version control system. It allows for cheap branching and merging, making it ideal for version control in software development.

### What is a Version Control System (VCS)?

A version control system keeps track of project changes and files in a central place, preventing code from being overridden. There are two types of VCS:
- **Centralized VCS**: A central server holds the main repository, and all users push/pull changes from it.
- **Distributed VCS**: Each developer has a complete copy of the project and its history on their machine. Examples: Git, Mercurial.

### Git vs GitHub

- **Git** is the version control system.
- **GitHub** is a web-based hosting service for Git repositories. It provides cloud-based access to your repositories.

## Git Workflow

1. **Working Directory**: You modify your code here.
2. **Staging Area**: You prepare your code for commit using `git add`.
3. **Repository**: Committed code is stored here.

### Basic Git Commands

- `git --version`: Check the installed version of Git.
- `git config --global user.name "Your Name"`: Set your Git username.
- `git config --global user.email "your.email@example.com"`: Set your Git email.
- `git init`: Initialize a new Git repository.
- `git status`: Check the status of your repository.
- `git add .`: Stage changes for commit.
- `git commit -m "message"`: Commit staged changes with a message.
- `git remote -v`: View remote repositories.
- `git remote add origin <repo-url>`: Add a remote repository.
- `git push -u origin main`: Push changes to GitHub.

### Branching and Merging

- `git branch`: View the list of branches.
- `git checkout <branch>`: Switch to a different branch.
- `git checkout -b <branch-name>`: Create a new branch and switch to it.
- `git merge <branch-name>`: Merge changes from one branch to another.
- `git diff`: View differences between branches.
- `git log --merge`: View commits causing merge conflicts.
- `git reset`: Reset to a previous commit.
- `git reset --mixed`: Undo changes in working directory/staging area.
- `git merge --abort`: Abort the merge process.
- `git branch -d <branch-name>`: Delete a branch.

### GitHub Pull Requests

A pull request (PR) is how you merge changes from one branch to another in GitHub. PRs allow collaborators to review and discuss changes before merging them into the main branch.

### Handling Merge Conflicts

Merge conflicts happen when Git cannot automatically decide which changes to keep. To resolve conflicts:
- Use `git status` to view conflicting files.
- Manually resolve conflicts in those files.
- Commit the resolved changes.

## SSH Key Setup for GitHub

1. Generate an SSH key:  
   `ssh-keygen -t ed25519 -C "your_email@example.com"`
2. Add the SSH key to GitHub.

### GitHub Pages: Hosting a Website

Follow these steps to host a website using GitHub:

1. **Initialize Git** in your project directory:
   ```bash
   git init
````

2. **Add files** to your Git repository:

   ```bash
   git add .
   ```

3. **Commit your files**:

   ```bash
   git commit -m "Initial commit of my website"
   ```

4. **Link to a GitHub repository**:

   ```bash
   git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git
   ```

5. **Push files to GitHub**:

   ```bash
   git push -u origin main
   ```

6. **Set up GitHub Pages**:

   * Go to the "Settings" tab of your GitHub repository.
   * Scroll to the "GitHub Pages" section.
   * Select the source branch (usually `main` or `master`).
   * Click "Save."
   * Your website will be available at `https://YOUR-USERNAME.github.io/REPO-NAME/`.

7. **Updating the website**:

   * Add and commit new changes:

     ```bash
     git add .
     git commit -m "Update website content"
     ```
   * Push updates to GitHub:

     ```bash
     git push origin main
     ```

## Conclusion

Git and GitHub are powerful tools for version control and collaboration in software development. With Git, you can track changes, collaborate with team members, and manage your project efficiently. GitHub adds the cloud-based hosting and collaboration features necessary for modern software development workflows.


