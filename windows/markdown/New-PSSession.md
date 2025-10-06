# New-PSSession Command

`New-PSSession` is a PowerShell command that creates a persistent connection, or session, to a local or remote computer. This session can be used to run commands without re-authenticating each time.

## Common Options

| Option          | Description                                                                 |
|-----------------|-----------------------------------------------------------------------------|
| `-ComputerName` | Specifies the name of the remote computer to connect to.                    |
| `-Credential`   | Provides user credentials for the remote session.                           |
| `-Port`         | Specifies the port to use for the connection. Defaults to 5985 (HTTP) or 5986 (HTTPS). |
| `-UseSSL`       | Indicates whether to use SSL to establish a connection.                     |
| `-Name`         | Assigns a friendly name to the session.                                     |

## Usage Examples

### Create a Session to a Remote Computer

```shell
$session = New-PSSession -ComputerName "Server01" -Credential (Get-Credential)
```

### Create a Session with SSL and a Custom Port

```shell
$session = New-PSSession -ComputerName "Server01" -UseSSL -Port 5986
```

### Assign a Name to the Session

```shell
$session = New-PSSession -ComputerName "Server01" -Name "MySession"
```

## Cheat Sheet

```shell
# Quick Reference
$session = New-PSSession -ComputerName "Server01" -Credential (Get-Credential)
$session = New-PSSession -ComputerName "Server01" -UseSSL
$session = New-PSSession -ComputerName "Server01" -Name "SessionName"
```

Use these commands to manage remote sessions efficiently!
