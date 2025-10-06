# Windows `cmd` Command

`cmd` is the command-line interpreter in Windows operating systems, used to execute entered commands. It can perform various tasks based on user input.

## Common Options

| Option          | Description                                           |
|-----------------|-------------------------------------------------------|
| `/C`            | Carries out the command specified by the string.     |
| `/K`            | Carries out the command specified and continues.     |
| `/S`            | Modifies how batch files are processed.              |
| `/Q`            | Turns echo off.                                      |
| `/D`            | Disables execution of AutoRun commands.              |
| `/A`            | Formats output as ANSI.                              |
| `/U`            | Formats output as Unicode.                           |
| `/T:fg`         | Sets foreground/background colors.                   |
| `/E:ON` or `/E:OFF` | Enables or disables command extensions.          |

## Usage Examples

### Run a Command

```sh
cmd /C dir
```

Executes the `dir` command and then terminates.

### Open Command Prompt and Keep it Open

```sh
cmd /K echo Hello, World!
```

Prints "Hello, World!" and stays open for further commands.

### Execute Batch Script Without AutoRun

```sh
cmd /D /C myscript.bat
```

Runs `myscript.bat` without executing AutoRun commands.

### Change Text Colors

```sh
cmd /T:0A
```

Sets text to bright green on a black background.

## Cheat Sheet

```plaintext
cmd /C [command]         # Execute command and close
cmd /K [command]         # Execute command and continue
cmd /S /C [command]      # Modify how batch files are processed
cmd /Q                   # Quiet mode (echo off)
cmd /D                   # Disable AutoRun
cmd /T:fg                # Set colors (f=foreground, g=background)
```
