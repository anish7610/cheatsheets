# `strace` Command in Linux

## Description

`strace` is a diagnostic, debugging, and instructional userspace utility for Linux. It is used to monitor the system calls made by a program and the signals received by the program. This tool is invaluable in troubleshooting, debugging, and learning how a program interacts with the system.

## Common Options

| Option      | Description                                                   |
|-------------|---------------------------------------------------------------|
| `-e trace=` | Trace only specified system calls.                            |
| `-o`        | Write trace output to a file.                                 |
| `-p`        | Attach to the process with the specified process ID.          |
| `-f`        | Trace child processes created by `fork` calls.                |
| `-c`        | Count time, calls, and errors for each system call.           |
| `-s`        | Specify the maximum string size to print (default is 32).     |

## Usage Examples

### Example 1: Trace All System Calls of a Command

```bash
strace ls
```

### Example 2: Trace Specific System Calls

Trace only `open` and `write` system calls:

```bash
strace -e trace=open,write ls
```

### Example 3: Write Output to a File

```bash
strace -o output.txt ls
```

### Example 4: Attach to a Running Process

Attach to a process with PID 1234:

```bash
strace -p 1234
```

### Example 5: Trace Child Processes

```bash
strace -f ./my_script.sh
```

### Example 6: Count System Call Stats

```bash
strace -c ls
```

## Cheat Sheet

```plaintext
strace [options] command
-e trace=open,write   # Trace specific system calls
-o output.txt         # Write output to a file
-p 1234               # Attach to process ID 1234
-f                    # Trace child processes
-c                    # Count system call stats
```
