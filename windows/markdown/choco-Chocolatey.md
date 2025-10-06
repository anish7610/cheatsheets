## Chocolatey (`choco`) Command

**Chocolatey** is a package manager for Windows that simplifies the process of installing, updating, and managing software via the command line.

### Common Options

| Option               | Explanation                                                  |
|----------------------|--------------------------------------------------------------|
| `install <package>`  | Installs the specified package.                              |
| `uninstall <package>`| Removes the specified package.                               |
| `update <package>`   | Updates the specified package to the latest version.         |
| `list`               | Lists all installed packages.                                |
| `find <package>`     | Searches for available packages.                             |
| `upgrade <package>`  | Upgrades the specified package or all if no package is specified. |

### Usage Examples

- **Install a Package:**
  ```sh
  choco install git
  ```

- **Uninstall a Package:**
  ```sh
  choco uninstall git
  ```

- **Update a Package:**
  ```sh
  choco update git
  ```

- **List All Installed Packages:**
  ```sh
  choco list --local-only
  ```

- **Find a Package:**
  ```sh
  choco find notepadplusplus
  ```

- **Upgrade All Packages:**
  ```sh
  choco upgrade all
  ```

### Cheat Sheet

```plaintext
choco install <package>   # Install a package
choco uninstall <package> # Uninstall a package
choco update <package>    # Update a package
choco list --local-only   # List installed packages
choco find <package>      # Search for a package
choco upgrade <package>   # Upgrade a package/all
```
