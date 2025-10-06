# `brew` Command in Linux

Homebrew is a package manager for Linux that allows you to install and manage software easily.

## Common Options

| Option            | Description                                        |
|-------------------|----------------------------------------------------|
| `install`         | Installs a package.                                |
| `update`          | Updates Homebrew itself and the formulae.          |
| `upgrade`         | Upgrades all outdated, unpinned packages.          |
| `list`            | Lists all installed packages.                      |
| `search`          | Searches for available packages.                   |
| `uninstall`       | Removes a package.                                 |
| `doctor`          | Checks the system for potential issues.            |
| `info`            | Displays information about a package.              |

## Usage Examples

### Install a Package
```bash
brew install wget
```

### Update Homebrew and Packages
```bash
brew update && brew upgrade
```

### Search for a Package
```bash
brew search python
```

### Uninstall a Package
```bash
brew uninstall wget
```

### List Installed Packages
```bash
brew list
```

### Get Help for a Command
```bash
brew help install
```

## Cheat Sheet

```plaintext
brew install <package>
brew update
brew upgrade
brew list
brew search <package>
brew uninstall <package>
brew doctor
brew info <package>
```
