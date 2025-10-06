## `Enter-PSSession` Command

`Enter-PSSession` is a PowerShell cmdlet used to start an interactive session with a remote computer. This allows you to execute commands as if you were logged on directly to the remote machine.

### Common Options

| Option              | Description                                                   |
|---------------------|---------------------------------------------------------------|
| `-ComputerName`     | Specifies the remote computer by name or IP address.          |
| `-Credential`       | Specifies a user account with which to perform the session.   |
| `-Port`             | Specifies the port number for the remote connection.          |
| `-UseSSL`           | Uses SSL to establish a secure connection to the remote host. |
| `-ConfigurationName`| Specifies an alternate session configuration on the host.     |

### Usage Examples

#### Connect to a Remote Computer

```powershell
Enter-PSSession -ComputerName "RemotePC"
```

#### Specify Credentials

```powershell
$cred = Get-Credential
Enter-PSSession -ComputerName "RemotePC" -Credential $cred
```

#### Use SSL for Secure Connection

```powershell
Enter-PSSession -ComputerName "RemotePC" -UseSSL
```

#### Connect Using a Specific Port

```powershell
Enter-PSSession -ComputerName "RemotePC" -Port 5986
```

#### Specify an Alternate Configuration

```powershell
Enter-PSSession -ComputerName "RemotePC" -ConfigurationName "CustomConfig"
```

### Cheat Sheet

```plaintext
# Basic connection
Enter-PSSession -ComputerName "RemotePC"

# With credentials
Enter-PSSession -ComputerName "RemotePC" -Credential (Get-Credential)

# Secure connection
Enter-PSSession -ComputerName "RemotePC" -UseSSL

# Specific port
Enter-PSSession -ComputerName "RemotePC" -Port 5986

# Custom configuration
Enter-PSSession -ComputerName "RemotePC" -ConfigurationName "CustomConfig"
```
