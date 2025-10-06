```markdown
# `expect` Command in Linux

## Description
`expect` is a Linux utility used for automating interactive applications. It scripts interactions by waiting for specific strings and sending programmed responses, making it ideal for tasks like automatic password entries and testing terminal applications.

## Common Options

| Option       | Description                                              |
|--------------|----------------------------------------------------------|
| `-c command` | Execute a single command.                                |
| `-f file`    | Execute commands from a file.                            |
| `--`         | Ends option parsing, useful for passing arguments.       |
| `-d`         | Enables debugging output, showing internal actions.      |
| `-i`         | Run in interactive mode, useful for debugging.           |
| `-v`         | Show version information.                                |

## Usage Examples

### Example 1: Automated SSH Login
```bash
#!/usr/bin/expect
spawn ssh user@remote_host
expect "password:"
send "your_password\r"
interact
```

### Example 2: FTP File Upload
```bash
#!/usr/bin/expect
spawn ftp remote_host
expect "Name"
send "username\r"
expect "Password"
send "your_password\r"
expect "ftp>"
send "put file.txt\r"
expect "ftp>"
send "bye\r"
```

### Example 3: Auto-responder in Chat
```bash
#!/usr/bin/expect
spawn chat_program
expect "Hello"
send "Hi, how can I help you?\r"
interact
```

## Cheat Sheet
```plaintext
expect <command>      # Run an interactive command automation
expect -c "<cmd>"     # Run single command directly
expect -f <file>      # Execute script file
send "<text>\r"       # Send text input
interact              # Allow user interaction after script
expect "<pattern>"    # Wait for pattern in output
```
```
