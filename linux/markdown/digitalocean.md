# DigitalOcean CLI (`doctl`)

The `doctl` command is a command-line interface for managing resources on the DigitalOcean platform. It allows you to interact with your DigitalOcean account and perform tasks like creating droplets, managing databases, and controlling networking components.

## Common Options

| Option                        | Explanation                                        |
|------------------------------ |---------------------------------------------------|
| `auth init`                   | Authenticate with your DigitalOcean account.      |
| `compute droplet create`      | Create a new droplet.                             |
| `compute droplet list`        | List all droplets in your account.                |
| `compute droplet delete`      | Delete an existing droplet by ID.                 |
| `compute ssh`                 | Connect to a droplet via SSH.                     |
| `database list`               | List all databases in your account.               |
| `vpc create`                  | Create a new Virtual Private Cloud.               |
| `vpc list`                    | List all VPCs in your account.                    |

## Usage Examples

### Authenticate with DigitalOcean

```bash
doctl auth init
```

### Create a New Droplet

```bash
doctl compute droplet create example-droplet --size s-1vcpu-1gb --image ubuntu-20-04-x64 --region nyc3
```

### List All Droplets

```bash
doctl compute droplet list
```

### Delete a Droplet

```bash
doctl compute droplet delete droplet-id
```

### Connect via SSH

```bash
doctl compute ssh droplet-name
```

### List All Databases

```bash
doctl database list
```

### Create a New VPC

```bash
doctl vpc create --name example-vpc --region nyc3
```

### List All VPCs

```bash
doctl vpc list
```

## Cheat Sheet

```plaintext
doctl auth init                       # Authenticate
doctl compute droplet create          # Create droplet
doctl compute droplet list            # List droplets
doctl compute droplet delete          # Delete droplet
doctl compute ssh                     # SSH to droplet
doctl database list                   # List databases
doctl vpc create                      # Create VPC
doctl vpc list                        # List VPCs
```
