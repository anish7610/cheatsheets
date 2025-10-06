### Packer Command in Linux

`packer` is a command-line tool used for creating machine and container images for multiple platforms from a single source configuration. It is commonly used in DevOps for automating the build of cloud images.

---

### Common Options

| Option               | Description                                                      |
|----------------------|------------------------------------------------------------------|
| `build`              | Build an image from a template.                                  |
| `inspect`            | Show components of a template.                                   |
| `init`               | Initialize a new configuration environment.                      |
| `validate`           | Check the validity of a template.                                |
| `version`            | Display the version of Packer.                                   |
| `-var 'key=value'`   | Set a variable value from the command line.                      |
| `-var-file=filename` | Load variables from a file.                                      |

---

### Usage Examples

#### Building an Image
```bash
packer build template.json
```

#### Inspecting a Template
```bash
packer inspect template.json
```

#### Validating a Template
```bash
packer validate template.json
```

#### Initializing a Packer Environment
```bash
packer init .
```

#### Setting Variables
```bash
packer build -var 'aws_region=us-west-1' template.json
```

---

### Cheat Sheet

```plaintext
Build image:        packer build template.json
Inspect template:   packer inspect template.json
Validate template:  packer validate template.json
Initialize:         packer init .
Set variable:       packer build -var 'key=value' template.json
Version:            packer version
```

---

This succinct guide should help you efficiently use `packer` for image-building tasks in your workflow.
