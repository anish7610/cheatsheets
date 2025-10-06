# QEMU Command Overview

`qemu` is a generic and open-source machine emulator and virtualizer. It allows you to run operating systems and programs on a virtual machine.

## Common Options

| Option                | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| `-drive file=FILE`    | Specifies the disk image file to use as a drive.                            |
| `-m SIZE`             | Sets the memory size for the virtual machine (e.g., `-m 512M` for 512 MB).  |
| `-cpu TYPE`           | Sets the CPU type for the virtual machine.                                  |
| `-netdev USER`        | Configures user-mode networking.                                            |
| `-cdrom FILE`         | Uses a file as a virtual CD-ROM.                                            |
| `-boot d`             | Boots from a specified device (e.g., `d` for CD-ROM).                       |
| `-nographic`          | Runs QEMU without a graphical output; useful for command-line only tasks.   |
| `-S`                  | Freezes the CPU at startup (useful for debugging).                          |
| `-gdb tcp::PORT`      | Opens a GDB server on the specified TCP port for debugging purposes.        |

## Usage Examples

### Basic VM Boot from Image

```bash
qemu-system-x86_64 -drive file=ubuntu.img -m 1G
```
Boots a virtual machine with 1 GB of RAM using `ubuntu.img` as the disk image.

### Boot from a CD-ROM

```bash
qemu-system-x86_64 -cdrom boot.iso -boot d
```
Launches a VM booting from `boot.iso` as a CD-ROM.

### Enable Networking

```bash
qemu-system-x86_64 -drive file=disk.img -netdev user,id=mynet0 -device e1000,netdev=mynet0
```
Boots a VM with user-mode networking using an `e1000` network device.

### Debugging with GDB

```bash
qemu-system-x86_64 -S -gdb tcp::1234
```
Starts a VM and waits for a GDB connection on TCP port 1234.

## Cheat Sheet

```plaintext
qemu-system-x86_64 -drive file=FILE -m SIZE -cpu TYPE -netdev USER [-cdrom FILE] [-boot d]
```
