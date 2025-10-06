# OpenStack Command

The `openstack` command-line interface (CLI) is used to manage and interact with OpenStack cloud resources. It allows users to perform tasks such as managing compute, network, identity, and more in an OpenStack environment.

## Common Options

| Option               | Description                                         |
|----------------------|-----------------------------------------------------|
| `--os-auth-url`      | URL for the OpenStack Identity API                  |
| `--os-project-name`  | Project name to scope to                           |
| `--os-username`      | Username for authentication                        |
| `--os-password`      | Password for authentication                        |
| `--os-region-name`   | The region to use                                   |
| `--os-domain-name`   | Domain name to scope to                             |
| `--debug`            | Print debugging output                             |
| `--help`             | Display help message for commands and options      |

## Usage Examples

### List All Servers
```bash
openstack server list
```

### Create a New Server
```bash
openstack server create --image IMAGE_ID --flavor FLAVOR_ID --network NETWORK_ID SERVER_NAME
```

### Delete a Server
```bash
openstack server delete SERVER_ID
```

### List Available Images
```bash
openstack image list
```

### Show Detailed Information about a Server
```bash
openstack server show SERVER_ID
```

## Cheat Sheet

```plaintext
# List servers
openstack server list

# Create server
openstack server create --image IMAGE_ID --flavor FLAVOR_ID --network NETWORK_ID SERVER_NAME

# Delete server
openstack server delete SERVER_ID

# List images
openstack image list

# Show server details
openstack server show SERVER_ID
```

Use these commands to efficiently interact with your OpenStack environment.
