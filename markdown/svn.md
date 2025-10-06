# SVN Command Overview

`svn` is a command-line tool for interacting with Subversion (SVN) repositories. It is used for version control of files and directories.

## Common Options

| Option            | Description                                           |
|-------------------|-------------------------------------------------------|
| `checkout` (`co`) | Check out a working copy from the repository.         |
| `update` (`up`)   | Bring changes from the repository into the working copy. |
| `commit` (`ci`)   | Send changes from your working copy to the repository.|
| `add`             | Add files and directories to your working copy.       |
| `status` (`st`)   | Print the status of working copy files and directories.|
| `diff`            | Display differences between files.                    |
| `log`             | Show the commit log messages.                         |
| `info`            | Display information about a local or remote item.     |
| `revert`          | Undo local changes to a file.                         |
| `merge`           | Merge changes into a working copy.                    |

## Usage Examples

### Checkout a Repository
```bash
svn checkout https://example.com/repo/project
```

### Update Working Copy
```bash
svn update
```

### Commit Changes
```bash
svn commit -m "Fixed bug #123"
```

### Add a File
```bash
svn add newfile.txt
```

### Check Status
```bash
svn status
```

### View Differences
```bash
svn diff
```

### View Commit Log
```bash
svn log
```

### Revert Changes
```bash
svn revert changedfile.txt
```

## SVN Cheat Sheet

```
svn co URL [DIR]      # Checkout
svn up                # Update
svn ci -m "Msg"       # Commit
svn add FILE          # Add file
svn st                # Status
svn diff              # Diff
svn log               # Log
svn revert FILE       # Revert file
```
