# `update-alternatives` Command

The `update-alternatives` command in Linux manages symbolic links for default commands or utilities. It allows multiple programs to provide the same functionality and lets the user switch between them.

## Common Options

| Option                   | Description                                                            |
|--------------------------|------------------------------------------------------------------------|
| `--install`              | Add a group of alternatives for a link.                                |
| `--config`               | Manually configure which alternative to use.                           |
| `--set`                  | Set a specific path as the active alternative for a link.              |
| `--remove`               | Remove a path from an alternative group.                               |
| `--display`              | Show information about the alternatives and their current status.      |
| `--list`                 | List all alternatives for a given name.                                |

## Usage Examples

### Installing and Configuring Alternatives

1. **Install a New Alternative:**
   ```bash
   sudo update-alternatives --install /usr/bin/editor editor /usr/bin/vim 100
   ```

2. **Manually Configure an Alternative:**
   ```bash
   sudo update-alternatives --config editor
   ```

3. **Set a Specific Alternative:**
   ```bash
   sudo update-alternatives --set editor /usr/bin/nano
   ```

### Removing and Displaying Alternatives

1. **Remove an Alternative:**
   ```bash
   sudo update-alternatives --remove editor /usr/bin/vim
   ```

2. **Display Information About Alternatives:**
   ```bash
   update-alternatives --display editor
   ```

3. **List All Alternatives for a Name:**
   ```bash
   update-alternatives --list editor
   ```

## Cheat Sheet

```plaintext
# Install new alternative
sudo update-alternatives --install LINK NAME PATH PRIORITY

# Configure alternatives
sudo update-alternatives --config NAME

# Set specific alternative
sudo update-alternatives --set NAME PATH

# Remove an alternative
sudo update-alternatives --remove NAME PATH

# Display alternative info
update-alternatives --display NAME

# List all alternatives
update-alternatives --list NAME
```
