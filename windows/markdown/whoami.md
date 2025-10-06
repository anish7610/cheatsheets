# `whoami` Command in Windows

## Description

The `whoami` command displays the username of the currently logged-in user. It's useful for verifying user identity and system permissions.

## Common Options

| Option       | Explanation                                      |
|--------------|--------------------------------------------------|
| `/all`       | Displays detailed user account information.      |
| `/user`      | Shows the user account name and security identifier (SID). |
| `/fqdn`      | Displays the fully qualified domain name.        |
| `/logonid`   | Displays the logon ID of the current user.       |

## Usage Examples

### Basic Username Display
```shell
whoami
```
*Outputs the current username.*

### Display Detailed Account Information
```shell
whoami /all
```
*Shows user's detailed information including privileges and group memberships.*

### Show User Account Name and SID
```shell
whoami /user
```
*Provides the username and security identifier.*

### Display Fully Qualified Domain Name
```shell
whoami /fqdn
```
*Shows the full domain name for the logged-in user.*

### Display Current User Logon ID
```shell
whoami /logonid
```
*Outputs the user's unique logon ID.*

## Cheat Sheet

```plaintext
whoami                  # Display current user
whoami /all             # Detailed account information
whoami /user            # User and SID
whoami /fqdn            # Fully qualified domain name
whoami /logonid         # Logon ID
```
