# Stop Command Overview

The `stop` command in Windows is used to terminate specific services that are running on the system. It's often utilized in scripts or command-line operations to manage Windows services effectively.

## Common Options

| Option        | Explanation                                    |
|---------------|------------------------------------------------|
| `/S`          | Specifies the remote system to stop a service. |
| `/U`          | Indicates the user context to run the command. |
| `/P`          | Provides the password for the user account.    |
| `/Y`          | Confirms the stop operation without prompts.   |

## Usage Examples

### Example 1: Stop a Local Service

```shell
net stop "ServiceName"
```
Stops a specified service on the local machine.

### Example 2: Stop a Remote Service Using Credentials

```shell
net stop "ServiceName" /S \\RemotePC /U UserName /P Password
```
Stops a service on a remote machine while providing user credentials.

### Example 3: Force Stop Without Prompts

```shell
net stop "ServiceName" /Y
```
Force stops a service without any confirmation prompts.

## Cheat Sheet

```shell
# Stop a local service
net stop "ServiceName"

# Stop a service on a remote machine
net stop "ServiceName" /S \\RemotePC /U UserName /P Password

# Force stop a service without prompts
net stop "ServiceName" /Y
```
