# Scoop Command on Windows

Scoop is a command-line installer for Windows that simplifies the process of installing and managing software. It automates downloads, installations, and updates of software, which can be particularly useful for developers and system administrators.

## Common Options

| Option         | Explanation                                                   |
|----------------|---------------------------------------------------------------|
| `scoop install` | Installs a specified application.                             |
| `scoop update`  | Updates installed applications to the latest versions.        |
| `scoop list`    | Lists all installed applications.                             |
| `scoop status`  | Shows the status of installed and outdated applications.      |
| `scoop uninstall` | Uninstalls a specified application.                         |
| `scoop search`  | Searches for an application in the available repositories.    |
| `scoop bucket`  | Manages application buckets (additional software sources).    |

## Usage Examples

### Install an Application
```bash
scoop install git
```

### Update All Applications
```bash
scoop update *
```

### List Installed Applications
```bash
scoop list
```

### Check Status of Applications
```bash
scoop status
```

### Uninstall an Application
```bash
scoop uninstall nodejs
```

### Search for an Application
```bash
scoop search python
```

### Add a Bucket and Install Software from It
```bash
scoop bucket add extras
scoop install vlc
```

## Cheat Sheet

```bash
scoop install <app>    # Install an app
scoop update *         # Update all apps
scoop list             # List all installed apps
scoop status           # Check app status
scoop uninstall <app>  # Uninstall an app
scoop search <app>     # Search for an app
scoop bucket add <name> # Add a software source
```
