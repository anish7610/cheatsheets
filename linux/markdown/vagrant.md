# Vagrant Command in Linux

Vagrant is a tool for building and managing virtualized development environments. It simplifies the setup process and integrates with various providers like VirtualBox, VMware, and more.

## Common Options

| Option       | Description                                         |
|--------------|-----------------------------------------------------|
| `up`         | Starts the virtual machine.                         |
| `halt`       | Stops the running virtual machine.                  |
| `destroy`    | Stops and deletes all traces of the virtual machine.|
| `status`     | Shows the current status of the virtual machine.    |
| `reload`     | Restarts the virtual machine, applying configuration changes. |
| `provision`  | Forces the provisioners to run again on a running VM. |
| `ssh`        | Connects to the virtual machine via SSH.            |
| `box`        | Manages Vagrant boxes.                              |

## Usage Examples

### Start a Virtual Machine

```bash
vagrant up
```

### Stop a Virtual Machine

```bash
vagrant halt
```

### Destroy a Virtual Machine

```bash
vagrant destroy
```

### Check the Status

```bash
vagrant status
```

### Connect via SSH

```bash
vagrant ssh
```

### Restart and Apply Changes

```bash
vagrant reload
```

### Run Provisioners

```bash
vagrant provision
```

## Quick Reference Cheat Sheet

```plaintext
vagrant up       # Start VM
vagrant halt     # Stop VM
vagrant destroy  # Destroy VM
vagrant status   # Check status
vagrant ssh      # SSH into VM
vagrant reload   # Restart with changes
vagrant provision # Reapply provisioners
vagrant box list # List available boxes
```

This guide provides essential commands and examples for using Vagrant effectively in a development environment.
