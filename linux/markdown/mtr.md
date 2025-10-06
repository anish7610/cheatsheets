# MTR Command Cheat Sheet

## Description

`mtr` (My Traceroute) is a network diagnostic tool that combines the functionality of `traceroute` and `ping` to display the route packets take to a network host and measure transit delay across an Internet Protocol (IP) network.

## Common Options

| Option          | Description                                                                  |
|-----------------|------------------------------------------------------------------------------|
| `-r`            | Generate report mode, suitable for capturing output for analysis.            |
| `-c <count>`    | Set the number of pings to send per hop.                                     |
| `-i <interval>` | Specify the interval between ICMP ECHO requests (default is one second).     |
| `-s <packetsize>` | Set the size of the packets used in the test.                               |
| `-n`            | Display numeric IP addresses only, skipping DNS lookup.                      |
| `-4`            | Force using IPv4 only.                                                       |
| `-6`            | Force using IPv6 only.                                                       |

## Usage Examples

### Example 1: Basic Usage
```bash
mtr google.com
```
*Trace the network path to `google.com` continuously.*

### Example 2: Report Mode
```bash
mtr -r -c 5 github.com
```
*Generate a report of 5 pings per hop to `github.com` and exit.*

### Example 3: Numeric Output
```bash
mtr -n reddit.com
```
*Display IP addresses without resolving hostnames for `reddit.com`.*

### Example 4: IPv4 Only
```bash
mtr -4 stackoverflow.com
```
*Force the use of IPv4 when tracing `stackoverflow.com`.*

### Example 5: Custom Packet Size
```bash
mtr -s 1500 -n example.com
```
*Send packets with a size of 1500 bytes to `example.com` with numeric IP output.*

## Quick Reference

```plaintext
mtr [options] <host>

-r         Report mode
-c <count> Count of pings per hop
-i <sec>   Interval between requests
-s <size>  Packet size
-n         Numeric IPs only
-4         Use IPv4 only
-6         Use IPv6 only
```
