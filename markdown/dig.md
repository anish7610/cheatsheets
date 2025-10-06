# `dig` Command in Linux

The `dig` (Domain Information Groper) command is used to query DNS name servers, troubleshooting DNS problems, or simply to look up information about domain names and IP addresses.

## Common Options

| Option          | Explanation                                                |
|-----------------|------------------------------------------------------------|
| `+short`        | Provides a brief answer without additional details.        |
| `+noall +answer`| Shows only the answer section of the query.                |
| `+stats`        | Includes statistics about the query in the output.         |
| `+trace`        | Traces the delegation path from the root name servers.     |
| `@server`       | Allows specifying a particular DNS server to query.        |
| `-x`            | Performs a reverse DNS lookup for an IP address.           |
| `+nodnssec`     | Disables DNSSEC authentication for the lookup.             |

## Usage Examples

### Basic Domain Lookup

```bash
dig example.com
```

### Short Answer Format

```bash
dig example.com +short
```

### Query a Specific DNS Server

```bash
dig @8.8.8.8 example.com
```

### Reverse DNS Lookup

```bash
dig -x 8.8.8.8 +short
```

### Trace a DNS Path

```bash
dig example.com +trace
```

### Display Only the Answer Section

```bash
dig example.com +noall +answer
```

### Include Query Statistics

```bash
dig example.com +stats
```

## Cheat Sheet

```
dig domain.com             # Basic DNS query
dig domain.com +short      # Short answer
dig @dns_server domain.com # Specific server
dig -x ip_address          # Reverse lookup
dig domain.com +trace      # DNS trace
dig domain.com +noall +answer # Answer only
```
