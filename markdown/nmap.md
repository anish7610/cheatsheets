# Nmap Command

**Nmap** (Network Mapper) is a powerful open-source tool for network discovery and security auditing. It is used to scan hosts and services on a computer network, thus creating a "map" of the network.

## Common Options

| Option          | Description                                                  |
|-----------------|--------------------------------------------------------------|
| `-sS`           | Initiates a TCP SYN scan (stealth scan).                     |
| `-sT`           | Performs a TCP connect scan.                                 |
| `-sU`           | Conducts a UDP scan.                                         |
| `-p <ports>`    | Specifies port(s) to scan, e.g., `-p 22,80,443` or `-p 1-65535`. |
| `-A`            | Enables OS detection, version detection, script scanning, and traceroute. |
| `-O`            | Enables OS detection.                                        |
| `-v`            | Increases verbosity level.                                   |
| `-Pn`           | Disables ping; treats all hosts as online.                   |
| `-T<0-5>`       | Sets timing template (0 is slow, 5 is fast).                 |
| `-oN`           | Outputs results in normal format to a file.                  |
| `-oX`           | Outputs results in XML format to a file.                     |
| `--script`      | Runs specific NSE scripts, e.g., `--script=http-title`.      |

## Usage Examples

### Basic TCP SYN Scan
```bash
nmap -sS example.com
```

### Scan Multiple Ports
```bash
nmap -p 22,80,443 example.com
```

### Scan All Ports
```bash
nmap -p- example.com
```

### OS and Version Detection
```bash
nmap -A example.com
```

### Disable Ping Discovery
```bash
nmap -Pn example.com
```

### Save Output to a File
```bash
nmap -oN output.txt example.com
```

### Fast Scan with Timing Template
```bash
nmap -T4 example.com
```

## Quick Reference Cheat Sheet

```plaintext
nmap -sS <target>                       # TCP SYN scan
nmap -p <ports> <target>                # Scan specific ports
nmap -A <target>                        # Enable OS and version detection
nmap -Pn <target>                       # Disable ping
nmap -oN output.txt <target>            # Save to file
nmap -T4 <target>                       # Faster scan
nmap --script=<script> <target>         # Run specific script
```
