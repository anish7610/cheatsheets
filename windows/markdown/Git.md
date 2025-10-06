# Git Command on Windows

Git is a distributed version control system often used to manage source code history. It allows multiple developers to collaborate efficiently on software projects.

## Common Options

| Option    | Description                                      |
|-----------|--------------------------------------------------|
| `clone`   | Copies a repository from a remote source.        |
| `init`    | Initializes a new Git repository.                |
| `status`  | Displays the state of the working directory.     |
| `add`     | Stages changes for the next commit.              |
| `commit`  | Records staged changes to the repository.        |
| `push`    | Uploads local commits to a remote repository.    |
| `pull`    | Fetches and merges changes from a remote repo.   |
| `branch`  | Lists, creates, or deletes branches.             |
| `checkout`| Switches branches or restores files.             |
| `merge`   | Combines changes from different branches.        |

## Usage Examples

### Clone a Repository

```bash
git clone https://github.com/user/repo.git
```

### Initialize a New Repository

```bash
git init
```

### Check Status

```bash
git status
```

### Add Changes to Staging

```bash
git add .
```

### Commit Changes

```bash
git commit -m "Add new feature"
```

### Push to Remote

```bash
git push origin main
```

### Pull Changes from Remote

```bash
git pull
```

### Create and Switch to a New Branch

```bash
git checkout -b new-feature
```

## Cheat Sheet

```plaintext
git clone URL        # Clone a repo
git init             # Initialize a repo
git status           # Show status
git add FILE         # Stage changes
git commit -m "MSG"  # Commit changes
git push             # Push to remote
git pull             # Pull from remote
git branch           # List branches
git checkout BRANCH  # Switch branches
git merge BRANCH     # Merge branches
```
