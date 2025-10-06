# `netsh http` Command

The `netsh http` command in Windows is used for configuring and managing HTTP settings for the HTTP Server API without needing to rely on GUI tools. It's primarily used for configuring SSL certificates, URL reservations, and logging.

## Common Options

| Option                      | Description                                            |
|-----------------------------|--------------------------------------------------------|
| `add sslcert`               | Adds a new SSL certificate binding.                    |
| `delete sslcert`            | Deletes an existing SSL certificate binding.           |
| `show sslcert`              | Displays the current SSL certificate bindings.         |
| `add urlacl`                | Reserves a URL namespace for a user or service.        |
| `delete urlacl`             | Deletes a reserved URL namespace.                      |
| `show urlacl`               | Displays reserved URL namespace entries.               |
| `add iplisten`              | Configures the IP addresses for the HTTP listener.     |
| `delete iplisten`           | Removes specified IP address from the HTTP listener.   |
| `show iplisten`             | Displays IP addresses for the HTTP listener.           |

## Usage Examples

### Add an SSL Certificate
To bind an SSL certificate to a specific IP and port:

```bash
netsh http add sslcert ipport=0.0.0.0:443 certhash=YOUR_CERT_HASH appid={YOUR_APP_ID}
```

### Delete an SSL Certificate
To remove an SSL binding:

```bash
netsh http delete sslcert ipport=0.0.0.0:443
```

### Reserve a URL Namespace
To reserve a URL for a specific user:

```bash
netsh http add urlacl url=http://+:8080/MyUri user=DOMAIN\User
```

### Show Reserved Namespaces
To list all reserved URL namespaces:

```bash
netsh http show urlacl
```

## Cheat Sheet

```plaintext
# Add SSL Certificate
netsh http add sslcert ipport=IP:PORT certhash=HASH appid={APP_ID}

# Delete SSL Certificate
netsh http delete sslcert ipport=IP:PORT

# Show SSL Certificates
netsh http show sslcert

# Reserve URL Namespace
netsh http add urlacl url=URL user=USER

# Delete URL Namespace
netsh http delete urlacl url=URL

# Show Reserved Namespaces
netsh http show urlacl

# Add IP Listener
netsh http add iplisten ipaddress=IP

# Delete IP Listener
netsh http delete iplisten ipaddress=IP

# Show IP Listeners
netsh http show iplisten
```

Use these commands to manage HTTP settings effectively through the command line, enhancing automation and scripting capabilities.
