# `taskkill` Command in Windows

`taskkill` is a command-line utility in Windows used to terminate tasks or processes.

## Common Options

| Option             | Description                                               |
|--------------------|-----------------------------------------------------------|
| `/PID <pid>`       | Specifies the PID of the process to be terminated.        |
| `/IM <imagename>`  | Specifies the process by image name to terminate.         |
| `/F`               | Forces the termination of the process.                    |
| `/T`               | Terminates the specified process and any child processes. |
| `/S <system>`      | Specifies the remote system on which to run the command.  |
| `/U <username>`    | Specifies the user context under which the command should run. |

## Usage Examples

Terminate a process by PID:

```bash
taskkill /PID 1234 /F
```

Terminate a process by image name:

```bash
taskkill /IM notepad.exe /F
```

Terminate a process and its child processes:

```bash
taskkill /PID 1234 /T
```

Terminate a process on a remote system:

```bash
taskkill /S remotePC /U admin /PID 1234 /F
```

## Cheat Sheet

```plaintext
taskkill /PID <pid> /F          # Force terminate by PID
taskkill /IM <name> /F          # Force terminate by name
taskkill /PID <pid> /T          # Terminate with child processes
taskkill /S <system> /U <user>  # Terminate on remote system
```
