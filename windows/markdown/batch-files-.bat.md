# Batch Files (.bat) in Windows

Batch files are script files containing a series of commands executed by the command-line interpreter (CMD.EXE). They automate tasks, execute scripts, or provide shortcuts for command sequences on Windows systems.

## Common Options

| Command    | Description                                  |
|------------|----------------------------------------------|
| `echo`     | Displays messages or toggles command echoing.|
| `pause`    | Pauses the execution, awaiting user input.   |
| `rem`      | Inserts comments in the batch file.          |
| `if`       | Executes commands based on conditions.       |
| `for`      | Loops through a set of files or commands.    |
| `set`      | Defines variables and their values.          |
| `call`     | Invokes another batch file or script.        |
| `exit`     | Exits the current script or command prompt.  |

## Usage Examples

### Basic Hello World

```batch
@echo off
echo Hello, World!
pause
```

### Create a Directory and Navigate

```batch
@echo off
mkdir C:\ExampleFolder
cd C:\ExampleFolder
echo You are now in C:\ExampleFolder
pause
```

### Conditional Execution

```batch
@echo off
if exist C:\test.txt (
    echo File exists.
) else (
    echo File does not exist.
)
pause
```

### Loop Through Files

```batch
@echo off
for %%f in (*.*) do (
    echo Processing file: %%f
)
pause
```

### Set and Use Variables

```batch
@echo off
set name=John
echo Hello, %name%
pause
```

## Cheat Sheet

```plaintext
@echo off        :: Disable command display
echo [message]   :: Display a message
pause            :: Wait for user input
rem [comment]    :: Add a comment
if [condition]   :: Conditional command execution
for %%var in (*) :: Loop through items
set [var=value]  :: Set a variable
call [batch]     :: Call another script
exit             :: Exit batch/script
```
