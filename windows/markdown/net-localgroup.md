## `net localgroup` Command

The `net localgroup` command is used to manage local group accounts on Windows. It allows you to view, create, modify, or delete local groups and manage user memberships.

### Common Options

| Option                          | Explanation                                             |
|---------------------------------|---------------------------------------------------------|
| `net localgroup`                | Lists all local groups on the system.                   |
| `net localgroup [groupname]`    | Displays details of a specific local group.             |
| `net localgroup [groupname] /add`         | Creates a new local group.                              |
| `net localgroup [groupname] /delete`      | Deletes a local group.                                  |
| `net localgroup [groupname] [username] /add`    | Adds a user to a specific local group.                  |
| `net localgroup [groupname] [username] /delete` | Removes a user from a specific local group.             |

### Usage Examples

#### List All Local Groups

```shell
net localgroup
```

#### Show Members of a Specific Group

```shell
net localgroup Administrators
```

#### Create a New Local Group

```shell
net localgroup Developers /add
```

#### Delete a Local Group

```shell
net localgroup Developers /delete
```

#### Add a User to a Local Group

```shell
net localgroup Administrators JohnDoe /add
```

#### Remove a User from a Local Group

```shell
net localgroup Administrators JohnDoe /delete
```

### Cheat Sheet

```markdown
- List groups: `net localgroup`
- Show group members: `net localgroup [groupname]`
- Create group: `net localgroup [groupname] /add`
- Delete group: `net localgroup [groupname] /delete`
- Add user to group: `net localgroup [groupname] [username] /add`
- Remove user from group: `net localgroup [groupname] [username] /delete`
```
