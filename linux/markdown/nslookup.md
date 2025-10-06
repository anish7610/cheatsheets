# `nslookup` Command Overview

The `nslookup` command-line utility is used to query Internet domain name servers. It finds the IP address associated with a domain name and vice versa, aiding in network diagnostics.

## Common Options

| Option          | Description                                              |
|-----------------|----------------------------------------------------------|
| `-type=`        | Specifies the query type: A (IPv4), AAAA (IPv6), MX, etc.|
| `-timeout=`     | Sets the timeout interval for a response.                |
| `-debug`        | Enables debugging mode for detailed output.              |
| `-retry=`       | Sets the number of retries for a query.                  |
| `-server`       | Specifies a DNS server to query.                         |

## Usage Examples

### Basic Domain Lookup
```bash
nslookup example.com
```

### Query a Specific Record Type (e.g., MX)
```bash
nslookup -type=MX example.com
```

### Use a Specific DNS Server
```bash
nslookup example.com 8.8.8.8
```

### Using Debug Mode
```bash
nslookup -debug example.com
```

### IPv6 Address Lookup
```bash
nslookup -type=AAAA example.com
```

## Cheat Sheet

```plaintext
Basic Usage: nslookup <domain>
Type Query: nslookup -type=<record_type> <domain>
Specific DNS: nslookup <domain> <dns_server>
Debug Mode: nslookup -debug <domain>
```
