# `letsencrypt` Command

`letsencrypt` is a command-line tool to manage SSL/TLS certificates through the Let's Encrypt Certificate Authority, primarily used for automating the acquisition and renewal of certificates.

## Common Options

| Option               | Description                                                   |
|----------------------|---------------------------------------------------------------|
| `-h`, `--help`       | Display help information on how to use the tool.              |
| `-v`, `--version`    | Show the version of the letsencrypt client.                   |
| `--agree-tos`        | Agree to the Let's Encrypt terms of service.                  |
| `-n`, `--non-interactive` | Run without prompting the user for input.               |
| `-d`, `--domain`     | Specify domain names for the certificate.                    |
| `--staging`          | Use the staging server for testing (avoid hitting rate limits).|
| `--renew-by-default` | Automatically renew the certificate when it is near expiry.   |
| `--webroot`          | Use the webroot path for authentication.                      |
| `--email`            | Email address for important account notifications.            |

## Usage Examples

### Obtain a Certificate for a Domain

```bash
letsencrypt certonly --webroot -w /var/www/html -d example.com --email you@example.com --agree-tos
```

### Renew an Existing Certificate

```bash
letsencrypt renew
```

### Test Renewal with Staging

```bash
letsencrypt renew --staging --dry-run
```

### Obtain a Certificate for Multiple Domains

```bash
letsencrypt certonly --webroot -w /var/www/html -d example.com -d www.example.com --email you@example.com --agree-tos
```

## Cheat Sheet

```plaintext
# Obtain a certificate
letsencrypt certonly --webroot -w /path -d domain.com --email user@example.com --agree-tos

# Renew all certificates
letsencrypt renew

# Test renewal (staging server, no changes)
letsencrypt renew --staging --dry-run
```

This should help you manage Let's Encrypt certificates efficiently and effectively!
