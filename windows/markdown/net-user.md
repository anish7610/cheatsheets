# `net user` Command in Windows

## Description

The `net user` command is used to manage user accounts on a Windows system. It allows administrators to add, modify, and delete user accounts, as well as set user properties.

## Common Options

| Option                  | Explanation                                              |
|-------------------------|----------------------------------------------------------|
| `username`              | Specifies the name of the user account to manage.        |
| `/add`                  | Adds a new user account.                                 |
| `/delete`               | Deletes a user account.                                  |
| `/active:{yes|no}`      | Activates or deactivates a user account.                 |
| `/fullname:"name"`      | Sets the full name of a user.                            |
| `/passwordchg:{yes|no}` | Permits or prevents the changing of a user password.     |
| `/logonpasswordchg:{yes|no}` | Requires or does not require a password change at next logon. |
| `/homedir:"path"`       | Sets the user's home directory.                          |

## Usage Examples

### Add a New User
```bash
net user newuser Password123 /add
```

### Delete a User
```bash
net user olduser /delete
```

### Change User Password
```bash
net user existinguser NewPass123
```

### Set User Full Name and Disable Account
```bash
net user sampleuser /fullname:"John Doe" /active:no
```

### Create User with Home Directory
```bash
net user testuser Password123 /add /homedir:"C:\Users\testuser"
```

## Cheat Sheet

```plaintext
# Add a new user
net user <username> <password> /add

# Delete a user
net user <username> /delete

# Change password
net user <username> <newpassword>

# Activate/deactivate user
net user <username> /active:{yes|no}

# Set full name
net user <username> /fullname:"Full Name"
```
