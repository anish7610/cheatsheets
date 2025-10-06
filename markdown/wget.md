# `wget` Command Overview

`wget` is a command-line utility for non-interactive downloading of files from the web. It supports HTTP, HTTPS, and FTP protocols.

## Common Options

| Option         | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `-O file`      | Write documents to `file`.                                                  |
| `-P prefix`    | Save files to `prefix/…`.                                                   |
| `-c`           | Continue getting a partially downloaded file.                               |
| `-b`           | Go to background after startup.                                             |
| `-q`           | Turn off Wget’s output.                                                     |
| `--limit-rate=`| Limit download speed, e.g., `--limit-rate=200k`.                            |
| `-r`           | Recursive download (downloads directories).                                 |
| `-l depth`     | Set the maximum recursion depth (inf or `0` for infinite).                  |
| `-np`          | Do not ever ascend to the parent directory when downloading recursively.    |
| `--user=`      | Specify the username for authentication.                                    |
| `--password=`  | Specify the password for authentication.                                    |

## Usage Examples

### Download a Single File

```bash
wget http://example.com/file.zip
```

### Download a File and Save with a Specific Name

```bash
wget -O newfile.zip http://example.com/file.zip
```

### Download a File to a Specific Directory

```bash
wget -P /path/to/directory http://example.com/file.zip
```

### Resume a Paused Download

```bash
wget -c http://example.com/largefile.zip
```

### Download Files in the Background

```bash
wget -b http://example.com/largefile.zip
```

### Limit Download Speed

```bash
wget --limit-rate=500k http://example.com/largefile.zip
```

### Download a Website Recursively

```bash
wget -r -l 1 http://example.com/
```

### Download with Credentials

```bash
wget --user=username --password=secret http://example.com/protectedfile.zip
```

## Cheat Sheet

```plaintext
wget [URL]                          # Download a file
wget -O [file] [URL]                # Save to specific filename
wget -P [prefix] [URL]              # Save to specific directory
wget -c [URL]                       # Resume download
wget -b [URL]                       # Background download
wget --limit-rate=[rate] [URL]      # Limit download speed
wget -r -np [URL]                   # Recursive download
wget --user=[user] --password=[pw] [URL]  # Authenticated download
```
