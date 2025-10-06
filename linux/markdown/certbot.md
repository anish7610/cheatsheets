# Certbot Command Overview

`certbot` is a client tool to automate the installation and renewal of free SSL/TLS certificates from the Let's Encrypt Certificate Authority. It makes securing web servers with HTTPS easy and efficient.

## Common Options

| Option             | Description                                                            |
|--------------------|------------------------------------------------------------------------|
| `-d`               | Specify the domains to include in the certificate.                     |
| `--nginx`          | Use the Nginx plugin to install the certificate automatically.         |
| `--apache`         | Use the Apache plugin to install the certificate automatically.        |
| `--standalone`     | Run a standalone web server for authentication.                        |
| `--manual`         | Obtain a certificate manually, useful for testing or custom setups.    |
| `--renew-by-default` | Automatically renew the certificate without user interaction.       |
| `--staging`        | Use the Let's Encrypt staging server for testing purposes.             |
| `--dry-run`        | Test the renewal process without making any actual changes.            |
| `-q`               | Run in quiet mode, suppressing most output.                            |

## Usage Examples

### Obtain a Certificate with Nginx

```bash
sudo certbot --nginx -d example.com -d www.example.com
```

### Obtain a Certificate with Apache

```bash
sudo certbot --apache -d example.com
```

### Renew All Certificates

```bash
sudo certbot renew
```

### Test Renewal Process

```bash
sudo certbot renew --dry-run
```

### Obtain a Certificate Manually

```bash
sudo certbot certonly --manual -d example.com
```

## Cheat Sheet

```plaintext
# Obtain certificate with Nginx
sudo certbot --nginx -d example.com

# Obtain certificate with Apache
sudo certbot --apache -d example.com

# Renew all certificates
sudo certbot renew

# Test renewal process
sudo certbot renew --dry-run

# Manual setup
sudo certbot certonly --manual -d example.com
```
