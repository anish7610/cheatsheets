# Windows `start` Command

The `start` command in Windows is used to open a new command prompt window, launch an application, or open a file. It allows users to specify how the program should be started, such as in a new window, minimized, or maximized.

## Common Options

| Option               | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| `/D path`            | Sets the specified path as the working directory.                           |
| `/I`                 | Passes the environment variables to the new process unmodified.             |
| `/MIN`               | Starts the window minimized.                                                |
| `/MAX`               | Starts the window maximized.                                                |
| `/WAIT`              | Waits for the started program to exit before continuing.                    |
| `/B`                 | Starts the application without creating a new window.                       |
| `title`              | Sets the title for the new command prompt window.                           |
| `command/program`    | Specifies the command or application to run.                                |
| `arguments`          | Additional arguments for the command or program.                            |

## Usage Examples

```bash
# Start Notepad
start notepad

# Open a URL in the default web browser
start https://www.example.com

# Open a file with its default program
start file.txt

# Start a program with a specific title
start "My Program" notepad.exe

# Run a command and wait for it to finish
start /WAIT notepad

# Start a program in a minimized window
start /MIN notepad

# Run a batch script with a specific working directory
start /D "C:\MyFolder" mybatch.bat
```

## Cheat Sheet

```plaintext
start [options] "title" command/program [arguments]
/D path    - Set working directory
/I         - Unmodified environment
/MIN       - Minimized window
/MAX       - Maximized window
/WAIT      - Wait for exit
/B         - No new window
```
