## Description

`iperf` is a tool for measuring the maximum TCP and UDP bandwidth performance between two systems by generating traffic and analyzing the speed of data transfer.

## Common Options

| Option        | Description                                                                            |
|---------------|----------------------------------------------------------------------------------------|
| `-s`          | Run `iperf` in server mode.                                                             |
| `-c <host>`   | Run `iperf` in client mode and connect to the specified server host.                    |
| `-u`          | Use UDP rather than TCP (the default) for data transfer.                                |
| `-p <port>`   | Specify a port to listen on or send traffic to. Defaults to 5201.                       |
| `-b <bandwidth>` | Set target bandwidth for UDP. Set in bits/sec (e.g., `1M` for 1 Megabit, `500K` for 500 Kilobits). |
| `-t <time>`   | Set the time in seconds to transmit for (default is 10 seconds).                        |
| `-i <interval>` | Set interval in seconds for periodic bandwidth reporting.                             |
| `-f <format>` | Set output to report in bits (`b`), bytes (`B`), kilobits (`k`), etc.                   |

## Usage Examples

1. **Run an iperf server:**

   ```bash
   iperf -s
   ```

2. **Run an iperf client to connect to a server at `192.168.1.2`:**

   ```bash
   iperf -c 192.168.1.2
   ```

3. **Run a UDP test from client to server:**

   ```bash
   iperf -c 192.168.1.2 -u
   ```

4. **Run a test with a 5 Mbits/sec UDP target bandwidth:**

   ```bash
   iperf -c 192.168.1.2 -u -b 5M
   ```

5. **Run a test with a 30-second duration:**

   ```bash
   iperf -c 192.168.1.2 -t 30
   ```

6. **Periodic bandwidth reporting every 2 seconds:**

   ```bash
   iperf -c 192.168.1.2 -i 2
   ```

## Cheat Sheet

```bash
# Server Mode
iperf -s

# Client Mode
iperf -c <host>

# UDP Test
iperf -c <host> -u

# Custom Port
iperf -c <host> -p <port>

# Set Bandwidth
iperf -c <host> -u -b <bandwidth>

# Custom Duration
iperf -c <host> -t <time>
```
