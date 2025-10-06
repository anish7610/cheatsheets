## Notepad Command in Windows

The `notepad` command is used to open the Notepad text editor from the command line. Notepad is a simple text editor for creating and editing plain text files.

### Common Options

| **Option**         | **Description**                                       |
|--------------------|-------------------------------------------------------|
| `filename`         | Opens the specified file in Notepad.                  |
| `/A`               | Forces an ANSI file to open (used with `filename`).   |
| `/P`               | Sends the file to the default printer without opening.|

### Usage Examples

1. **Open a File in Notepad**

   ```bash
   notepad example.txt
   ```

2. **Create a New File**

   ```bash
   notepad newfile.txt
   ```

3. **Open a File as ANSI**

   ```bash
   notepad example.txt /A
   ```

4. **Print a File**

   ```bash
   notepad example.txt /P
   ```

### Cheat Sheet

```bash
# Open a file
notepad filename

# Create or edit a file
notepad newfile.txt

# Open as ANSI
notepad filename /A

# Print a file
notepad filename /P
```
