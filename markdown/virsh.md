# `virsh` Command Overview

`virsh` is a command-line interface tool for managing virtual machines using the libvirt library. It provides a way to create, edit, start, stop, and manage virtual machines and their resources.

## Common Options

| Option          | Description                                                                 |
|-----------------|-----------------------------------------------------------------------------|
| `list`          | Lists all running virtual machines.                                          |
| `start <vm>`    | Starts a specified virtual machine.                                          |
| `shutdown <vm>` | Gracefully shuts down a specified virtual machine.                           |
| `destroy <vm>`  | Forces a stop on a specified virtual machine (similar to pulling the plug).  |
| `create <xml>`  | Creates a new virtual machine from an XML file.                              |
| `define <xml>`  | Defines a new VM without starting it, from an XML file.                      |
| `undefine <vm>` | Removes the specified virtual machine from the configuration.                |
| `console <vm>`  | Connects to a virtual machine console.                                       |
| `dominfo <vm>`  | Displays detailed information about a specified virtual machine.             |
| `edit <vm>`     | Opens the XML configuration file of a virtual machine for editing.           |

## Usage Examples

### List Running Virtual Machines

```bash
virsh list
```

### Start a Virtual Machine

```bash
virsh start my-vm
```

### Shut Down a Virtual Machine

```bash
virsh shutdown my-vm
```

### Force Stop a Virtual Machine

```bash
virsh destroy my-vm
```

### Create a New Virtual Machine from XML

```bash
virsh create my-vm.xml
```

### Define a Virtual Machine Without Starting

```bash
virsh define my-vm.xml
```

### Connect to a Virtual Machine Console

```bash
virsh console my-vm
```

## Cheat Sheet

```plaintext
virsh list                     # List running VMs
virsh start <vm>               # Start a VM
virsh shutdown <vm>            # Shutdown a VM
virsh destroy <vm>             # Force stop (destroy) a VM
virsh create <xml>             # Create VM from XML
virsh define <xml>             # Define VM without starting
virsh undefine <vm>            # Remove VM configuration
virsh console <vm>             # Connect to VM console
virsh dominfo <vm>             # VM details
virsh edit <vm>                # Edit VM XML
```
