# Git and GitHub Guide

This repository contains a comprehensive guide on Git and GitHub, covering key concepts, workflows, and commands.

---

## 🧰 What is Git?

- **Free** and **open source**
- **Scalable**, **superfast**, and **local**
- **Cheap branching and merging**
- A **Version Control System (VCS)** that tracks changes in your code/projects.

---

## 🔍 Version Control System (VCS)

A system that:
- Keeps track of project files and changes.
- Prevents overwriting code.
- Centralized vs. Distributed:

### Centralized VCS
- One main server, all developers push/pull code from it.
- Collaborative and synchronized.
- Suitable for small projects.

### Distributed VCS
- Complete project copy on every machine.
- Enables mirroring and offline work.
- Examples: Git, Mercurial

---

## 🌐 GitHub

- A **web-based hosting service** for Git repositories.
- **Cloud-based** collaboration tool.
- Cannot be used without Git.

---

## 🖥️ Git Workflow

### Local Git Workflow:
```text
Working Directory → (git add) → Staging Area → (git commit) → Repository → (git push)
````

### GitHub Workflow:

```text
Write Code → Commit → Pull Request
```

---

## 📁 Key Git Concepts

* **Repository**: Project folder tracked by Git.
* **Index / Staging Area**: Temporary area to format/review code before committing.
* **Blob (Binary Large Object)**: Stores file data and metadata.
* **Tree**: Represents directory structure containing blobs/subdirectories.
* **Branching**: Create separate lines of development.

  * `master`: Default branch.
  * `feature`: For adding new features.
  * `hotfix`: For urgent fixes.

---

## 🌿 Branching & Merging

* `git branch`: Check current branch.
* `git checkout`: Switch between branches.
* `git checkout -b branch_name`: Create and switch to a new branch.
* `git merge branch_name`: Merge changes into current branch.
* `git diff`: Compare changes between branches.

---

## ⚠️ Merge Conflicts

* Occurs when Git cannot determine which change to keep.
* Use:

  * `git log --merge` to see conflicting commits.
  * `git merge --abort` to cancel merge.
  * `git reset` or `git reset --mixed` to undo changes.

---

## 🔐 SSH Key Setup

1. Run: `ssh-keygen -t ed25519 -C "your_email@example.com"`
2. Set name and passphrase.
3. Copy the `.pub` file content.
4. Add it to your GitHub SSH keys.

---

## 💡 GitHub Issues

* Track bugs, tasks, and enhancements.
* Each issue has a number (e.g., #3).
* To close: include `closes #3` in pull request description.

---

## 🚀 Host a Website Using GitHub Pages

1. **Initialize Repository**
   `git init`

2. **Add Files**
   `git add .`

3. **Commit**
   `git commit -m "Initial commit of my website"`

4. **Link Remote Repo**
   `git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git`

5. **Push Code**
   `git push -u origin main`

6. **Enable GitHub Pages**

   * Go to repo > Settings > Pages
   * Choose branch (e.g., `main`)
   * Save

7. **Update Website**

   ```bash
   git add .
   git commit -m "Update website content"
   git push origin main
   ```

Your site will be live at:
`https://YOUR-USERNAME.github.io/REPO-NAME/`

---

## 🛠️ Common Git Commands

```bash
git --version                       # Check Git version
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

git init                            # Initialize repo
git status                          # Check status
git add .                           # Stage all changes
git commit -m "message"             # Commit with message
git remote add origin <URL>         # Add remote repo
git push -u origin main             # Push to GitHub

git branch                          # List branches
git checkout branch_name            # Switch branches
git checkout -b new_branch          # Create + switch
git merge branch_name               # Merge branch
git diff                            # View changes

git reset                           # Undo changes
git merge --abort                   # Cancel merge
git branch -d branch_name           # Delete branch
```

---

## 📦 Stash

Temporarily save your changes for later use:

```bash
git stash           # Stash changes
git stash apply     # Reapply stashed changes
```

---
