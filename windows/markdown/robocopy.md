# `robocopy` Command in Windows

`robocopy` (Robust File Copy) is a command-line utility for copying files and directories in Windows. It is designed to handle complex copying requirements, such as mirroring directories, copying only updated files, and managing network interruptions.

## Common Options

| Option       | Description                                                |
|--------------|------------------------------------------------------------|
| `/S`         | Copies subdirectories, excluding empty ones.               |
| `/E`         | Copies all subdirectories, including empty ones.           |
| `/COPY:copyflags` | Specifies the file properties to copy (e.g., data, attributes). |
| `/MOV`       | Moves files and deletes them from the source.              |
| `/MIR`       | Mirrors a directory tree (equivalent to `/E` + `/PURGE`).  |
| `/PURGE`     | Deletes destination files and directories that no longer exist in the source. |
| `/XJ`        | Excludes junction points, often used to prevent infinite loops. |
| `/R:n`       | Sets the number of retries on failures (default: 1 million).|
| `/W:n`       | Sets the wait time between retries in seconds (default: 30).|
| `/LOG:file`  | Redirects output to a log file, appending to the file if it exists. |
| `/MT[:n]`    | Copies using multiple threads (default is 8). Maximum is 128. |

## Usage Examples

1. **Basic File Copy:**

   ```shell
   robocopy C:\Source C:\Destination
   ```

2. **Mirror Directories:**

   ```shell
   robocopy C:\Source C:\Destination /MIR
   ```

3. **Copy with Logging:**

   ```shell
   robocopy C:\Source C:\Destination /S /LOG:C:\robocopy.log
   ```

4. **Copy and Move Files:**

   ```shell
   robocopy C:\Source C:\Destination /MOV
   ```

5. **Multithreaded Copy:**

   ```shell
   robocopy C:\Source C:\Destination /MT:16
   ```

## Cheat Sheet

```plaintext
BASIC COPY        robocopy src dst
MIRROR            robocopy src dst /MIR
COPY SUBDIRS      robocopy src dst /E
MOVE FILES        robocopy src dst /MOV
WITH LOG          robocopy src dst /LOG:file
MULTITHREAD       robocopy src dst /MT:n
```
