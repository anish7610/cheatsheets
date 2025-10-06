# `hostname` Command in Linux

The `hostname` command is used to display or set the system's network name or hostname.

## Common Options

| Option      | Description                                             |
|-------------|---------------------------------------------------------|
| `-s, --short`  | Display the short hostname (without domain).            |
| `-f, --fqdn, --long` | Display the full hostname (fully qualified domain name). |
| `-i, --ip-address`  | Display the network address(es) associated with the hostname. |
| `-I, --all-ip-addresses`  | Display all network addresses of the host.          |
| `-d, --domain`  | Display the name of the DNS domain.                         |
| `-y, --yp, --nis` | Show the NIS (Network Information Services) domain name. |
| `-V, --version`  | Show the program's version information.                 |
| `-h, --help`     | Display help information.                                |

## Usage Examples

### Display the Current Hostname

```bash
hostname
```

### Show the Short Hostname

```bash
hostname -s
```

### Display the Full Qualified Domain Name

```bash
hostname -f
```

### List All IP Addresses

```bash
hostname -I
```

### Set a Temporary Hostname

```bash
sudo hostname new-hostname
```

### Show the DNS Domain Name

```bash
hostname -d
```

## Cheat Sheet

```markdown
# Display current hostname
hostname

# Short hostname
hostname -s

# Full hostname (FQDN)
hostname -f

# All IP addresses
hostname -I

# Set hostname (temporary)
sudo hostname [new-name]
```
