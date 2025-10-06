# Linux Command: `upgrade`

## Description

The `upgrade` command is used in package management on Linux systems to update installed packages to their latest versions. It is typically part of package management tools like `apt`, `dnf`, or `yum`. The specific behavior and options can vary based on the package manager.

## Common Options (for `apt-get`)

| Option         | Description                                     |
|----------------|-------------------------------------------------|
| `-y`           | Automatically answer 'yes' to prompts.          |
| `--dry-run`    | Simulate the upgrade without making changes.    |
| `--with-new-pkgs` | Installs new packages as well as upgrading existing ones. |
| `--force-yes`  | Force yes to prompts, even if potentially harmful. |
| `-q`           | Quiet mode; suppress normal output.             |

## Usage Examples

### Basic Upgrade

```bash
sudo apt-get upgrade
```

### Automatically Confirm Prompts

```bash
sudo apt-get upgrade -y
```

### Simulate Upgrade

```bash
sudo apt-get upgrade --dry-run
```

### Upgrade with New Packages

```bash
sudo apt-get upgrade --with-new-pkgs
```

## Cheat Sheet

```bash
# Basic upgrade
sudo apt-get upgrade

# Auto-confirm
sudo apt-get upgrade -y

# Simulate upgrade
sudo apt-get upgrade --dry-run

# Upgrade with new packages
sudo apt-get upgrade --with-new-pkgs
```
