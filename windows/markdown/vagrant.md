# Vagrant Command in Windows

**Description**

Vagrant is a command-line tool used for creating and managing virtualized development environments. It simplifies the setup and configuration of virtual machines, ensuring consistent environments across development, staging, and production.

## Common Options

| Option          | Description                                             |
|-----------------|---------------------------------------------------------|
| `up`            | Starts and provisions the Vagrant environment.          |
| `halt`          | Stops the running Vagrant machine.                      |
| `reload`        | Restarts the Vagrant machine, applying any changes.     |
| `destroy`       | Stops and deletes all traces of the Vagrant machine.    |
| `status`        | Shows the state of the Vagrant environment.             |
| `ssh`           | Connects to the machine via SSH.                        |
| `provision`     | Applies changes to the running Vagrant machine.         |
| `box add`       | Adds a new Vagrant box.                                 |
| `box list`      | Lists available Vagrant boxes.                          |
| `box remove`    | Removes a Vagrant box.                                  |
| `init`          | Initializes a Vagrant environment with a Vagrantfile.   |

## Usage Examples

```bash
# Start a Vagrant environment using a Vagrantfile
vagrant up

# Stop a running Vagrant machine
vagrant halt

# Restart and apply configuration changes
vagrant reload

# Delete the Vagrant machine
vagrant destroy

# Check the status of the Vagrant environment
vagrant status

# SSH into a Vagrant machine
vagrant ssh

# Add a new Vagrant box
vagrant box add ubuntu/bionic64

# List all Vagrant boxes
vagrant box list

# Remove a Vagrant box
vagrant box remove ubuntu/bionic64

# Initialize a new Vagrantfile in the current directory
vagrant init hashicorp/bionic64
```

## Quick Reference Cheat Sheet

```plaintext
vagrant up        # Start VM
vagrant halt      # Stop VM
vagrant reload    # Restart VM
vagrant destroy   # Remove VM
vagrant status    # VM status
vagrant ssh       # Access VM
vagrant provision # Apply changes
vagrant init      # Setup Vagrantfile
```
