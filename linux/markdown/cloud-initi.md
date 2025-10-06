# `cloud-init` Command Overview

`cloud-init` is a utility used in cloud computing to initialize and configure cloud instances during boot. It handles initial configurations such as setting up SSH keys, network configurations, and executing user scripts.

## Common Options

| Option                | Description                                                        |
|-----------------------|--------------------------------------------------------------------|
| `init`                | Initializes cloud-init and runs all initialization stages.         |
| `status`              | Displays the current status of cloud-init.                         |
| `single`              | Runs a single specific module, such as `users-groups`.             |
| `query`               | Fetches specific configuration keys from cloud-init metadata.      |
| `modules`             | Executes specific cloud-init modules to customize instance setup.  |
| `devel`               | Provides developer-related subcommands for debugging purposes.     |
| `clean`               | Removes cloud-init artifacts for redeployment or testing.          |

## Usage Examples

### Initialize Cloud-Init

```bash
sudo cloud-init init
```
This command triggers all stages of cloud initialization.

### Check Cloud-Init Status

```bash
cloud-init status
```
Provides an overview of the current status and result of cloud-init operations.

### Run a Specific Module

```bash
sudo cloud-init single -n users-groups
```
Executes the `users-groups` module to configure users and groups.

### Query Metadata

```bash
cloud-init query ds.meta_data.local_hostname
```
Fetches the local hostname from the instance's metadata.

### Clean Artifacts for Redeployment

```bash
sudo cloud-init clean
```
Removes all cloud-init cache and logs for fresh initialization.

## Cheat Sheet

```plaintext
Initialize:        sudo cloud-init init
Status:            cloud-init status
Run Module:        sudo cloud-init single -n <module-name>
Query Metadata:    cloud-init query <key>
Clean Artifacts:   sudo cloud-init clean
```
