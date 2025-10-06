# `msiexec` Command

`msiexec` is a command-line utility in Windows used for installing, configuring, and handling `.msi` (Microsoft Installer) packages.

## Common Options

| Option                  | Description                                           |
|-------------------------|-------------------------------------------------------|
| `/i <package>`          | Installs or configures the specified product.         |
| `/x <package>`          | Uninstalls the specified product.                     |
| `/qn`                   | Quiet mode, no user interface during install/uninstall. |
| `/qb`                   | Basic UI during install/uninstall.                    |
| `/l*vx <logfile>`       | Enables verbose logging, writing to the specified file.|
| `/a <package>`          | Installs a product on the network.                    |
| `/f <package>`          | Repairs the installed package.                        |

## Usage Examples

### Install a Package

```bash
msiexec /i example.msi /qb
```

### Uninstall a Package

```bash
msiexec /x example.msi /qn
```

### Install with Logging

```bash
msiexec /i example.msi /l*vx install.log
```

### Repair an Installation

```bash
msiexec /f example.msi /qn
```

## Cheat Sheet

```plaintext
Install:    msiexec /i <package> /qn
Uninstall:  msiexec /x <package> /qn
Log:        msiexec /i <package> /l*vx <logfile>
Repair:     msiexec /f <package> /qn
Quiet Mode: /qn (no UI), /qb (basic UI)
```
