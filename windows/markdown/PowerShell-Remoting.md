## PowerShell Remoting

PowerShell Remoting allows you to run commands on remote computers. It is built on top of Windows Remote Management (WinRM) and enables you to administer multiple computers from a single command prompt.

### Common Options

| Option         | Description                                                         |
|----------------|---------------------------------------------------------------------|
| `-ComputerName`| Specify the target computer for the command.                        |
| `-Credential`  | Use alternate credentials for remote execution.                     |
| `-Port`        | Specify a custom port for the remote connection (default is 5985).  |
| `-UseSSL`      | Use SSL for the connection.                                         |
| `-ScriptBlock` | Define a block of script to be executed on the remote machine.      |
| `-ThrottleLimit`| Limit the number of concurrent connections.                         |

### Usage Examples

#### Invoke a Command on a Remote Computer

```powershell
Invoke-Command -ComputerName "Server01" -ScriptBlock { Get-Process }
```

#### Use Alternate Credentials

```powershell
$cred = Get-Credential
Invoke-Command -ComputerName "Server01" -Credential $cred -ScriptBlock { Restart-Service "Spooler" }
```

#### Run a Command on Multiple Computers

```powershell
Invoke-Command -ComputerName "Server01", "Server02" -ScriptBlock { Get-Service }
```

#### Use SSL for Secure Connection

```powershell
Invoke-Command -ComputerName "Server01" -UseSSL -ScriptBlock { Get-EventLog "System" }
```

### Compact Cheat Sheet

```plaintext
# Basic Command
Invoke-Command -ComputerName "Server" -ScriptBlock { <Command> }

# Using Credentials
$cred = Get-Credential
Invoke-Command -ComputerName "Server" -Credential $cred -ScriptBlock { <Command> }

# Multiple Machines
Invoke-Command -ComputerName "Server1", "Server2" -ScriptBlock { <Command> }

# Secure Connection
Invoke-Command -ComputerName "Server" -UseSSL -ScriptBlock { <Command> }
```
