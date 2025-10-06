# `tracert` Command in Windows

`tracert` is a command-line utility used to trace the path that packets take from your computer to a destination network address. It helps in diagnosing network routing issues by reporting the series of routers (hops) through which data travels.

## Common Options

| Option       | Description                                               |
|--------------|-----------------------------------------------------------|
| `-d`         | Do not resolve addresses to hostnames.                    |
| `-h <maxhops>` | Maximum number of hops to search for target (default is 30). |
| `-w <timeout>` | Timeout in milliseconds to wait for each reply.         |
| `-4`         | Force using IPv4.                                         |
| `-6`         | Force using IPv6.                                         |

## Examples

### Basic Usage

Trace the path to a website:

```bash
tracert example.com
```

### Using IPv4 Only

Force IPv4 to trace to a domain:

```bash
tracert -4 example.com
```

### Limit Hops

Trace with a maximum of 15 hops:

```bash
tracert -h 15 example.com
```

### No Hostname Resolution

Trace without resolving hostnames:

```bash
tracert -d example.com
```

### Set Timeout

Increase timeout to 5000 milliseconds:

```bash
tracert -w 5000 example.com
```

## Cheat Sheet

```plaintext
tracert <destination>               # Basic trace
tracert -4 <destination>            # Use IPv4
tracert -6 <destination>            # Use IPv6
tracert -d <destination>            # No hostname resolution
tracert -h <maxhops> <destination>  # Set max hops
tracert -w <timeout> <destination>  # Set reply timeout
```
