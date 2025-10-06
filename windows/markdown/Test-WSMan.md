# Test-WSMan Command

`Test-WSMan` is a Windows PowerShell command used to test the functionality and availability of the Windows Remote Management (WinRM) service on a local or remote machine.

## Common Options

| Option             | Explanation                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| `-ComputerName`    | Specifies the remote computer to test. Defaults to the local computer.     |
| `-Port`            | Specifies the port to connect to (default is 5985 for HTTP, 5986 for HTTPS).|
| `-Credential`      | Specifies a user account to use when connecting to the remote computer.    |
| `-UseSSL`          | Indicates that the connection should use HTTPS.                             |
| `-Authentication`  | Specifies the authentication method to use (e.g., `Default`, `Kerberos`).   |

## Usage Examples

### Test the Local Machine

```powershell
Test-WSMan
```

### Test a Remote Machine

```powershell
Test-WSMan -ComputerName "remote-server"
```

### Test a Remote Machine Over HTTPS

```powershell
Test-WSMan -ComputerName "remote-server" -UseSSL
```

### Test with Specific Port

```powershell
Test-WSMan -ComputerName "remote-server" -Port 5985
```

### Test with Specific Credentials

```powershell
$cred = Get-Credential
Test-WSMan -ComputerName "remote-server" -Credential $cred
```

## Cheat Sheet

```plaintext
# Test local machine
Test-WSMan

# Test remote machine
Test-WSMan -ComputerName "remote-server"

# Use HTTPS
Test-WSMan -ComputerName "remote-server" -UseSSL

# Use specific port
Test-WSMan -ComputerName "remote-server" -Port 5985

# Use credentials
$cred = Get-Credential
Test-WSMan -ComputerName "remote-server" -Credential $cred
```
