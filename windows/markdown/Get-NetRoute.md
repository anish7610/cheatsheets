# Get-NetRoute Command in Windows

`Get-NetRoute` is a Windows PowerShell command used to display IP routing table entries on local or remote computers. It helps in managing and troubleshooting network configurations.

## Common Options

| Option                  | Explanation                                                   |
|-------------------------|---------------------------------------------------------------|
| `-InterfaceIndex`       | Specifies the index of the network interface.                 |
| `-InterfaceAlias`       | Specifies the alias of the network interface.                 |
| `-DestinationPrefix`    | Filters routes by destination IP prefix.                      |
| `-NextHop`              | Filters routes by the next hop IP address.                    |
| `-AddressFamily`        | Specifies whether to show IPv4 or IPv6 routes (`IPv4` or `IPv6`). |
| `-PolicyStore`          | Indicates where the policy is stored (e.g., `PersistentStore`).|

## Usage Examples

### View All Routes

```shell
Get-NetRoute
```

### Filter by Interface Index

```shell
Get-NetRoute -InterfaceIndex 12
```

### Filter by Destination Prefix

```shell
Get-NetRoute -DestinationPrefix "0.0.0.0/0"
```

### Display IPv6 Routes Only

```shell
Get-NetRoute -AddressFamily IPv6
```

## Cheat Sheet

```plaintext
# Show all routes
Get-NetRoute

# Filter by interface index
Get-NetRoute -InterfaceIndex <Index>

# Filter by destination
Get-NetRoute -DestinationPrefix "<CIDR>"

# Display IPv4/IPv6 routes
Get-NetRoute -AddressFamily <IPv4|IPv6>
```
