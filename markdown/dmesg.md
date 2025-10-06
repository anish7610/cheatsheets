# `dmesg` Command in Linux

The `dmesg` command displays the kernel ring buffer messages, which contain information about hardware operations and system diagnostics.

## Common Options

| Option     | Explanation                                      |
|------------|--------------------------------------------------|
| `-C`       | Clears the ring buffer.                          |
| `-c`       | Clears the buffer after printing.                |
| `-H`       | Provides human-readable timestamps.              |
| `-L`       | Uses the locale for human-readable timestamps.   |
| `-T`       | Shows the timestamp in human-readable format.    |
| `-w`       | Waits for new messages continuously like `tail`. |
| `-x`       | Decodes facility and level numbers.              |

## Usage Examples

### Display Kernel Messages

```bash
dmesg
```

### Clear the Kernel Buffer

```bash
dmesg -C
```

### Follow Newer Kernel Messages

```bash
dmesg -w
```

### Show Human-Readable Timestamps

```bash
dmesg -T
```

### Decode Facility and Level Numbers

```bash
dmesg -x
```

## Cheat Sheet

```plaintext
dmesg        # Display messages
dmesg -C     # Clear messages
dmesg -w     # Follow new messages
dmesg -T     # Human-readable timestamps
dmesg -x     # Decode numbers
```
