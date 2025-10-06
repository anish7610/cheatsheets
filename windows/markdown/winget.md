# `winget` Command

`winget` is a command-line utility for managing software packages on Windows. It allows users to discover, install, upgrade, remove, and configure applications directly from the command line.

## Common Options

| Option         | Description                                                                    |
|----------------|--------------------------------------------------------------------------------|
| `install`      | Installs a specified application by name or ID.                                |
| `show`         | Displays information about a specified application.                             |
| `search`       | Searches for applications in the repository.                                    |
| `list`         | Lists all installed applications on the system.                                 |
| `upgrade`      | Upgrades an installed application or all applications if no name is specified.  |
| `uninstall`    | Uninstalls a specified application.                                             |
| `source`       | Manages the sources of the packages.                                            |

## Usage Examples

### Install an Application

```bash
winget install "Mozilla Firefox"
```

### Search for an Application

```bash
winget search "Visual Studio Code"
```

### Show Application Details

```bash
winget show "Google Chrome"
```

### List Installed Applications

```bash
winget list
```

### Upgrade All Applications

```bash
winget upgrade --all
```

### Uninstall an Application

```bash
winget uninstall "Spotify"
```

## Cheat Sheet

```plaintext
winget install <app>    # Install an application
winget search <app>     # Search for an app
winget show <app>       # Show app details
winget list             # List installed apps
winget upgrade --all    # Upgrade all apps
winget uninstall <app>  # Uninstall an app
```
