# `nmcli` Command Overview

`nmcli` is a command-line tool used to manage NetworkManager, a service that manages network connections on Linux systems. It provides commands to display, configure, and troubleshoot network settings.

## Common Options

| Option          | Description                                               |
|-----------------|-----------------------------------------------------------|
| `device`        | Manage network interfaces (e.g., show, connect, disconnect). |
| `connection`    | Handle network connections (e.g., up, down, modify, delete). |
| `general`       | Display or modify general NetworkManager status.          |
| `networking`    | Enable or disable networking.                             |
| `radio`         | Control wireless radio switches.                          |
| `agent`         | Run nmcli's secret agent or polkit agent.                 |
| `monitor`       | Monitor NetworkManager changes.                           |

## Usage Examples

### Display all network connections

```bash
nmcli connection show
```

### Connect to a specific network

```bash
nmcli device wifi connect "Network_SSID" password "your_password"
```

### Disconnect a device

```bash
nmcli device disconnect wlan0
```

### Bring up a connection

```bash
nmcli connection up "Connection_Name"
```

### Bring down a connection

```bash
nmcli connection down "Connection_Name"
```

### Add a new Wi-Fi connection

```bash
nmcli connection add type wifi ifname wlan0 ssid "Network_SSID" -- wifi-sec.key-mgmt wpa-psk wifi-sec.psk "your_password"
```

### Display device status

```bash
nmcli device status
```

### Turn off networking

```bash
nmcli networking off
```

### Turn on wireless radio

```bash
nmcli radio wifi on
```

## Cheat Sheet

```plaintext
# List all connections
nmcli con show

# Connect to Wi-Fi
nmcli dev wifi connect "SSID" password "PWD"

# Disconnect device
nmcli dev disconnect wlan0

# Bring up/down a connection
nmcli con up "NAME"
nmcli con down "NAME"

# Add Wi-Fi connection
nmcli con add type wifi ifname wlan0 ssid "SSID" -- wifi-sec.key-mgmt wpa-psk wifi-sec.psk "PWD"

# Device status
nmcli dev status

# Toggle networking
nmcli networking off/on

# Toggle Wi-Fi radio
nmcli radio wifi off/on
```
