## Flatpak Command

Flatpak is a versatile tool for building, distributing, and running sandboxed desktop applications on Linux. It allows you to install apps, manage their runtimes, and handle versions in a more secure and straightforward manner.

### Common Options

| Option               | Description                                                 |
|----------------------|-------------------------------------------------------------|
| `install <repo> <package>` | Install a package from a specified repository            |
| `run <package>`      | Run an installed package                                     |
| `update`             | Update all installed Flatpak packages                        |
| `list`               | List all installed Flatpak packages                          |
| `uninstall <package>`| Remove an installed Flatpak package                          |
| `info <package>`     | Display detailed information about a package                 |
| `search <term>`      | Search for packages matching a search term                   |

### Usage Examples

#### Install an Application
Install the GIMP application from Flathub:
```bash
flatpak install flathub org.gimp.GIMP
```

#### Run an Application
Run the installed GIMP application:
```bash
flatpak run org.gimp.GIMP
```

#### Update All Packages
Update all installed Flatpak applications and runtimes:
```bash
flatpak update
```

#### List Installed Packages
List all currently installed Flatpak applications:
```bash
flatpak list
```

#### Uninstall an Application
Remove the GIMP application:
```bash
flatpak uninstall org.gimp.GIMP
```

#### Search for Applications
Search for packages related to "editor":
```bash
flatpak search editor
```

### Cheat Sheet

```markdown
# Flatpak Cheat Sheet

# Install a package
flatpak install <repo> <package>

# Run a package
flatpak run <package>

# Update packages
flatpak update

# List installed packages
flatpak list

# Uninstall a package
flatpak uninstall <package>

# Search for packages
flatpak search <term>
```
