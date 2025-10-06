## `curl` Command Overview

The `curl` command is a versatile tool for transferring data using various network protocols. It is widely used for its simplicity and support of multiple protocols like HTTP, HTTPS, FTP, and more.

### Common Options

| Option          | Description                                                   |
|-----------------|---------------------------------------------------------------|
| `-o <file>`     | Write output to a file instead of stdout.                     |
| `-O`            | Save file with the remote name.                               |
| `-L`            | Follow redirects.                                             |
| `-I`            | Fetch headers only.                                           |
| `-X <command>`  | Specify the request method to use.                            |
| `-d <data>`     | Send specified data in POST request.                          |
| `-H <header>`   | Pass custom header to the server.                             |
| `-u <user:pass>`| Set user and password for server authentication.              |
| `-k`            | Allow connections to SSL sites without certificates.          |

### Usage Examples

**Download a File:**

```bash
curl -O http://example.com/file.txt
```

**Follow Redirects:**

```bash
curl -L http://short.url
```

**Fetch Only the Headers:**

```bash
curl -I http://example.com
```

**POST Data:**

```bash
curl -d "name=John" -X POST http://example.com/form
```

**Custom Headers:**

```bash
curl -H "Authorization: Bearer token" http://example.com/resource
```

**Authentication:**

```bash
curl -u username:password http://example.com/login
```

### Compact Cheat Sheet

```plaintext
curl [options] [URL...]
-o <file>  # Save to file
-L         # Follow redirects
-I         # Fetch headers only
-d <data>  # POST data
-H <hdr>   # Add header
-u <u:p>   # User:pass auth
```
