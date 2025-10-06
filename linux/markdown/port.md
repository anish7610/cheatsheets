## `port` Command in Linux

The `port` command is generally used on macOS with MacPorts, a package management system for installing open-source software. In Linux, a similar tool might be `apt`, `yum`, or `dnf`.

### Common Options

| Option            | Description                                              |
|-------------------|----------------------------------------------------------|
| `list outdated`   | Lists installed ports that have newer versions available.|
| `upgrade outdated`| Upgrades all outdated ports to the latest version.       |
| `search [name]`   | Searches for available ports with the specified name.    |
| `install [port]`  | Installs the specified port.                             |
| `uninstall [port]`| Uninstalls the specified port.                           |

### Usage Examples

1. **List Outdated Ports**
   ```bash
   port list outdated
   ```

2. **Upgrade Outdated Ports**
   ```bash
   port upgrade outdated
   ```

3. **Search for a Port**
   ```bash
   port search vim
   ```

4. **Install a Port**
   ```bash
   port install vim
   ```

5. **Uninstall a Port**
   ```bash
   port uninstall vim
   ```

### Cheat Sheet

```plaintext
port list outdated        # List ports with updates
port upgrade outdated     # Update all outdated ports
port search [name]        # Search for a port
port install [name]       # Install a port
port uninstall [name]     # Remove a port
```

Note: Replace `[name]` with the specific port/package name.
