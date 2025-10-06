# `nslookup` Command in Windows

## Description

`nslookup` is a network administration command-line tool used for querying Domain Name System (DNS) to obtain domain name or IP address mapping or other DNS records.

## Common Options

| Option              | Description                                             |
|---------------------|---------------------------------------------------------|
| `<hostname>`        | Resolve the IP address of a given domain name.          |
| `<IP address>`      | Find the domain name associated with an IP address.     |
| `server <hostname>` | Specify a DNS server to use for the query.              |
| `set type=record`   | Specify the type of DNS record to query (e.g., A, MX).  |
| `exit`              | Exit nslookup interactive mode.                         |

## Usage Examples

### Look Up Domain IP Address

```
nslookup example.com
```

### Reverse Lookup an IP Address

```
nslookup 93.184.216.34
```

### Specify a DNS Server

```
nslookup example.com 8.8.8.8
```

### Query a Specific DNS Record Type

```
nslookup -type=MX example.com
```

### Interactive Mode

```sh
nslookup
> server 8.8.8.8
> set type=A
> example.com
> exit
```

## Cheat Sheet

```sh
# Lookup domain IP
nslookup example.com

# Reverse IP lookup
nslookup 93.184.216.34

# Use specific DNS server
nslookup example.com 8.8.8.8

# Query specific DNS record type
nslookup -type=MX example.com
```
