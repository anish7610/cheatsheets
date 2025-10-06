# `update` Command in Linux

The `update` command is not a standard Linux command. It is often related to package management in some distributions, where users execute commands to refresh package lists or upgrade packages. The exact command and functionality vary between package managers (e.g., `apt`, `dnf`, `yum`).

## Common Usage with `apt`

On Debian-based systems like Ubuntu, `update` functionality is often accessed via:

- `apt update`: Updates the list of available packages and their versions, but does not install or upgrade any packages.

## Common Options with `apt update`

| Option             | Description                                  |
|--------------------|----------------------------------------------|
| `-y`               | Assume "yes" as an answer to prompts.        |
| `--allow-releaseinfo-change` | Allow changing release information. |
| `-q`               | Operate quietly.                             |
| `--list-cleanup`   | Automatically manage unused lists.           |

## Usage Examples

### Update Package List

```bash
sudo apt update
```

### Update Package List Quietly

```bash
sudo apt update -q
```

### Update with Release Info Change Allowed

```bash
sudo apt update --allow-releaseinfo-change
```

## Cheat Sheet

```bash
# Update package list
sudo apt update

# Update quietly
sudo apt update -q

# Allow release info change
sudo apt update --allow-releaseinfo-change
```
