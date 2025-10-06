# Linux Command: `ln`

The `ln` command is used to create links between files. There are two types of links: hard links and symbolic (soft) links. Hard links point directly to the data on disk, whereas symbolic links point to another filename.

## Common Options

| Option | Description                                |
|--------|--------------------------------------------|
| `-s`   | Create a symbolic (soft) link.             |
| `-f`   | Force the creation of a link, removing existing destination files. |
| `-v`   | Verbosely list files being processed.      |
| `-t`   | Specify the target directory.              |
| `-n`   | Treat destination that is a symbolic link to a directory as a normal file. |

## Usage Examples

### Create a Hard Link
```bash
ln original.txt hardlink.txt
```

### Create a Symbolic Link
```bash
ln -s original.txt symlink.txt
```

### Forcefully Create a Symbolic Link
```bash
ln -sf original.txt symlink.txt
```

### Verbose Mode
```bash
ln -sv original.txt symlink.txt
```

### Create a Link in a Directory
```bash
ln -s original.txt /path/to/directory/
```

### Create a Link with Target Directory
```bash
ln -s -t /path/to/directory/ original.txt
```

## Cheat Sheet

```markdown
# Create a hard link
ln source target

# Create a symbolic link
ln -s source target

# Force create a symbolic link
ln -sf source target

# Verbosely create a link
ln -sv source target

# Link to a directory
ln -s -t directory/ source
```
