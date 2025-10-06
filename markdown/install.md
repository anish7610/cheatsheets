# Linux `install` Command

The `install` command is used to copy files and set attributes. It's typically used to install programs or files in a specific location with set permissions.

## Common Options

| Option      | Description                                           |
|-------------|-------------------------------------------------------|
| `-c`        | Ignored; for compatibility with other versions.       |
| `-d`        | Create directories instead of copying files.          |
| `-m` MODE   | Set the permission mode (like `chmod`).               |
| `-o` OWNER  | Set the owner of the copied files.                    |
| `-g` GROUP  | Set the group of the copied files.                    |
| `-p`        | Preserve the original file's timestamps.              |

## Usage Examples

### Install a Program or Script
```bash
install -m 755 myscript.sh /usr/local/bin/
```
Copies `myscript.sh` to `/usr/local/bin/` with executable permissions.

### Create a Directory Structure
```bash
install -d /var/www/html/mywebsite
```
Creates the directory path `/var/www/html/mywebsite`.

### Copy a File and Set Ownership
```bash
install -o user -g group myfile.txt /home/user/documents/
```
Copies `myfile.txt` to `/home/user/documents/` and sets ownership to `user:group`.

## Cheat Sheet

```plaintext
install [options] SOURCE DEST
install -d DIRECTORY
install -m MODE FILE DEST
install -o OWNER -g GROUP FILE DEST
```
