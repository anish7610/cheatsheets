# `useradd` Command Overview

The `useradd` command in Linux is used to create a new user account on the system. It's a low-level utility that modifies system files to set up the user environment.

## Common Options

| Option      | Description                                                   |
|-------------|---------------------------------------------------------------|
| `-m`        | Create the user's home directory.                             |
| `-d`        | Specify an alternative home directory path.                   |
| `-c`        | Add a comment field, often used for the full name.            |
| `-s`        | Define the user's login shell.                                |
| `-g`        | Specify the initial group.                                    |
| `-G`        | Specify additional groups the user should belong to.          |
| `-u`        | Define the user ID (UID) for the account.                     |
| `-e`        | Set the account expiration date (YYYY-MM-DD format).          |
| `-f`        | Set the number of days after password expiration until the account is disabled. |
| `-p`        | Pre-encrypted password (use with caution).                    |

## Usage Examples

### Create a New User with a Home Directory
```bash
sudo useradd -m username
```

### Create a User with a Specific Shell and Comment
```bash
sudo useradd -m -s /bin/bash -c "John Doe" username
```

### Create a User with a Home Directory Path
```bash
sudo useradd -m -d /custom/home username
```

### Create a User with Specific Groups
```bash
sudo useradd -m -G sudo,developers username
```

### Create a User with a Specific UID and Expiration Date
```bash
sudo useradd -m -u 1050 -e 2023-12-31 username
```

## Cheat Sheet

```bash
# Basic user creation with home directory
sudo useradd -m username

# Specify login shell and comment
sudo useradd -m -s /bin/bash -c "Full Name" username

# Set home directory path and additional groups
sudo useradd -m -d /custom/home -G group1,group2 username

# Define UID and expiration date
sudo useradd -m -u UID -e YYYY-MM-DD username
```
