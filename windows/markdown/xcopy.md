# `xcopy` Command in Windows

`xcopy` is a command-line utility in Windows used to copy files and directories, including subdirectories. It's more powerful than the basic `copy` command, making it suitable for backing up and mirroring files and directories.

## Common Options

| Option         | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `/S`           | Copies directories and subdirectories except empty ones.                    |
| `/E`           | Copies all subdirectories, including empty ones.                            |
| `/H`           | Copies hidden and system files as well.                                     |
| `/C`           | Continues copying files even if errors occur.                               |
| `/I`           | If destination does not exist and copying more than one file, assume it's a directory. |
| `/Y`           | Suppresses prompting to confirm overwriting a file.                         |
| `/D:mm-dd-yyyy`| Copies files changed on or after the specified date.                        |
| `/R`           | Overwrites read-only files.                                                 |

## Usage Examples

### Backup a Directory
Copy all files and subdirectories from `C:\Data` to `D:\Backup`, including empty directories.

```bash
xcopy C:\Data D:\Backup /E /H /C /I
```

### Copy Updated Files Only
Copy files from `C:\Project` to `D:\ProjectBackup` that have been updated since March 1, 2023.

```bash
xcopy C:\Project D:\ProjectBackup /D:03-01-2023 /E /C /I
```

### Clone a Directory Structure
Copy the directory structure of `C:\Template` without the files.

```bash
xcopy C:\Template D:\EmptyStructure /T /E
```

### Copy with Overwrite Confirmation Disabled
Copy everything from `C:\Source` to `D:\Destination`, suppressing overwrite confirmations.

```bash
xcopy C:\Source D:\Destination /E /H /C /I /Y
```

## Cheat Sheet

```plaintext
xcopy source destination [options]

/S  - Copy subdirectories except empty
/E  - Copy all subdirectories including empty
/H  - Include hidden/system files
/C  - Ignore errors
/I  - Assume destination is directory
/Y  - Suppress overwrite prompts
/D:date - Copy changed files since date
/R  - Overwrite read-only files
```
