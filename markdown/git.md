# Git Command Overview

`git` is a distributed version control system used to track changes in source code during software development. It enables multiple developers to work together on code in a non-linear fashion.

## Common Options

| Option                 | Explanation                                            |
|------------------------|--------------------------------------------------------|
| `git init`             | Initialize a new Git repository.                       |
| `git clone <repo>`     | Clone an existing repository.                          |
| `git status`           | Show the working directory status.                     |
| `git add <file>`       | Add a file to the staging area.                        |
| `git commit -m "<msg>"`| Commit staged changes with a message.                  |
| `git push`             | Push committed changes to a remote repository.         |
| `git pull`             | Fetch and merge changes from a remote repository.      |
| `git branch`           | List, create, or delete branches.                      |
| `git checkout <branch>`| Switch to a specified branch.                          |
| `git merge <branch>`   | Merge a branch into the current branch.                |
| `git log`              | Show the commit history.                               |
| `git diff`             | Show changes between commits, commit and working tree, etc. |
| `git reset <file>`     | Remove a file from the staging area.                   |
| `git rm <file>`        | Delete a file from the working directory and stage it. |

## Usage Examples

### Initialize a Repository

```bash
git init
```

### Clone a Repository

```bash
git clone https://github.com/user/repo.git
```

### Check Status

```bash
git status
```

### Add Files to Staging

```bash
git add example.txt
```

### Commit Changes with a Message

```bash
git commit -m "Add example file"
```

### Push to Remote

```bash
git push origin main
```

### Pull Latest Changes

```bash
git pull origin main
```

### Create and Switch to a New Branch

```bash
git branch new-feature
git checkout new-feature
```

### Merge a Branch

```bash
git checkout main
git merge new-feature
```

## Quick Cheat Sheet

```plaintext
git init                # Start a new repository
git clone <repo>        # Copy a remote repository
git status              # Check status
git add <file>          # Stage changes
git commit -m "<msg>"   # Commit with message
git push                # Send changes to remote
git pull                # Update local with remote changes
git branch              # Manage branches
git checkout <branch>   # Change branch
git merge <branch>      # Merge branch
git log                 # View commit history
git diff                # Show differences
```
