# `apt-cache` Command

`apt-cache` is a command-line tool used to query the APT (Advanced Package Tool) package cache in Debian-based systems. It provides information about available packages, helping users understand installation options and dependencies.

## Common Options

| Option      | Description                                                 |
|-------------|-------------------------------------------------------------|
| `search`    | Search the package list for a term.                         |
| `show`      | Display detailed information about a package.               |
| `depends`   | Show package dependencies.                                  |
| `rdepends`  | Show reverse dependencies.                                  |
| `policy`    | Display the installed and candidate versions of a package.  |
| `stats`     | Show statistics about the package cache.                    |

## Usage Examples

### Search for a Package

Search for a package containing the term "editor":

```bash
apt-cache search editor
```

### Show Package Details

Display detailed information about the package `vim`:

```bash
apt-cache show vim
```

### Check Dependencies

List dependencies for the package `curl`:

```bash
apt-cache depends curl
```

### Find Reverse Dependencies

Find out what packages depend on `libcurl3`:

```bash
apt-cache rdepends libcurl3
```

### Check Package Policy

Show installed and candidate versions for `wget`:

```bash
apt-cache policy wget
```

### View Cache Statistics

Display statistics about the package cache:

```bash
apt-cache stats
```

## Cheat Sheet

```bash
# Search for packages
apt-cache search [term]

# Show package details
apt-cache show [package]

# List package dependencies
apt-cache depends [package]

# Show reverse dependencies
apt-cache rdepends [package]

# Check version policy
apt-cache policy [package]

# View cache statistics
apt-cache stats
```

Use these commands for efficient package management and exploration on your Debian-based system.
