# Linux `sed` Command

`sed` (Stream Editor) is a powerful utility used for parsing and transforming text in a data stream. It is often used for text substitution, deletion, and basic text manipulations.

## Common Options

| Option      | Description                                             |
|-------------|---------------------------------------------------------|
| `-e`        | Add the script to the commands to be executed           |
| `-i`        | Edit files in place (modify the original file)          |
| `-n`        | Suppress automatic printing of pattern space            |
| `-f`        | Add the script file to the commands to be executed      |
| `-r`        | Use extended regular expressions                        |

## Usage Examples

### Substitute text

Replace "foo" with "bar" in a file:

```bash
sed 's/foo/bar/' file.txt
```

### Edit a file in place

Replace "foo" with "bar" in the file and save changes:

```bash
sed -i 's/foo/bar/' file.txt
```

### Delete lines containing a pattern

Remove lines containing "delete me":

```bash
sed '/delete me/d' file.txt
```

### Print lines matching a pattern

Print only lines that contain "pattern":

```bash
sed -n '/pattern/p' file.txt
```

### Use extended regular expressions

Insert a space after every digit:

```bash
sed -r 's/([0-9])/\1 /g' file.txt
```

## Cheat Sheet

```markdown
# Basic substitution
sed 's/old/new/' file.txt

# In-place edit
sed -i 's/old/new/' file.txt

# Delete lines with pattern
sed '/pattern/d' file.txt

# Print lines with pattern
sed -n '/pattern/p' file.txt

# Extended regex
sed -r 's/(regex)/\1/' file.txt
```

Use `sed` to quickly and effectively perform text stream editing tasks on files directly from the command line.
