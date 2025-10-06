# `usermod` Command

The `usermod` command in Linux is used to modify a user's account details, including change of login name, user ID, home directory, and more.

## Common Options

| Option         | Description                                                |
|----------------|------------------------------------------------------------|
| `-c <comment>` | Change the user’s comment field (GECOS).                   |
| `-d <dir>`     | Change the user's home directory.                          |
| `-e <date>`    | Set the expiration date for the user account.              |
| `-g <group>`   | Change the user's primary group.                           |
| `-G <group>`   | Add the user to supplementary groups.                      |
| `-L`           | Lock the user account.                                     |
| `-U`           | Unlock the user account.                                   |
| `-l <login>`   | Change the user's login name.                              |
| `-p <password>`| Change the user's encrypted password.                      |
| `-s <shell>`   | Change the user's login shell.                             |
| `-u <UID>`     | Change the user’s ID.                                      |

## Usage Examples

### Change the User's Home Directory

```bash
usermod -d /new/home/dir username
```

### Lock a User Account

```bash
usermod -L username
```

### Add a User to Supplementary Groups

```bash
usermod -G group1,group2 username
```

### Change a User's Login Name

```bash
usermod -l newname username
```

### Set an Expiration Date for a User Account

```bash
usermod -e 2023-12-31 username
```

## Cheat Sheet

```markdown
usermod -c "New Comment" username     # Change comment
usermod -d /home/newdir username      # Change home directory
usermod -l newlogin username          # Change login name
usermod -G group1,group2 username     # Add to groups
usermod -L username                   # Lock account
usermod -U username                   # Unlock account
```
