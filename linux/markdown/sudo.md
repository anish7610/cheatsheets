# `sudo` Command in Linux

`sudo` allows permitted users to run commands as the superuser or another user, as specified in the `sudoers` file.

## Common Options

| Option     | Description                                          |
|------------|------------------------------------------------------|
| `-h`       | Display help message and exit.                       |
| `-l`       | List the allowed (and forbidden) commands for the user. |
| `-u [user]`| Execute the command as the specified user.           |
| `-k`       | Invalidate the user's cached credentials.            |
| `-b`       | Run the command in the background.                   |
| `-s`       | Run the shell specified by the `SHELL` environment variable.  |

## Usage Examples

### Run a Command as Superuser
```bash
sudo apt update
```

### Run a Command as a Different User
```bash
sudo -u username ls /home/username
```

### List User Privileges
```bash
sudo -l
```

### Run a Command in the Background
```bash
sudo -b ./long-running-script.sh
```

### Clear Cached Credentials
```bash
sudo -k
```

## Cheat Sheet

```plaintext
sudo [options] command
sudo -u [user] command
sudo -l
sudo -b command
sudo -k
```
