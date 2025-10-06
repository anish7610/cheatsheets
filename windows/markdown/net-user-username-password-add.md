# `net user [username] [password] /add` Command

## Description

The `net user` command in Windows is used to manage user accounts on a computer. The specific command `net user [username] [password] /add` is used to create a new user account with the specified username and password.

## Common Options

| Option         | Explanation                                                   |
|----------------|---------------------------------------------------------------|
| `/add`         | Adds a new user account.                                      |
| `/delete`      | Deletes a user account.                                       |
| `/active:{yes|no}` | Activates or deactivates the account.                    |
| `/expires:{date|never}` | Sets an expiration date for the account.            |
| `/fullname:"<name>"` | Sets the full name of the user.                        |
| `/passwordchg:{yes|no}` | Allows or disallows password changes by the user.   |
| `/passwordreq:{yes|no}` | Specifies if a password is required.               |

## Usage Examples

### Add a Simple User
```bash
net user johndoe P@ssw0rd123 /add
```

### Add a User with Full Name and No Password Expiration
```bash
net user johndoe P@ssw0rd123 /add /fullname:"John Doe" /passwordchg:no
```

### Add a User and Prevent Them from Changing Password
```bash
net user johndoe P@ssw0rd123 /add /passwordchg:no
```

### Add a User with Account Expiration
```bash
net user johndoe P@ssw0rd123 /add /expires:12/31/2023
```

## Cheat Sheet

```bash
# Add user with password: net user [username] [password] /add
# Delete user: net user [username] /delete
# Add user, no password change: net user [username] [password] /add /passwordchg:no
# Add user with expiration: net user [username] [password] /add /expires:[date]
```
