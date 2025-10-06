# `perf` Command Overview

`perf` is a performance analysis tool in Linux that provides insights into system and application behavior. It's useful for profiling and monitoring performance events.

## Common Options

| Option        | Description                                               |
|---------------|-----------------------------------------------------------|
| `stat`        | Collects and displays performance counter statistics.     |
| `record`      | Records performance data for later analysis.              |
| `report`      | Analyzes and displays data collected with `perf record`.  |
| `list`        | Lists available performance events.                       |
| `top`         | Displays real-time performance data similar to `top`.     |
| `annotate`    | Provides inline assembly-level analysis of recorded data. |

## Usage Examples

### Displaying Performance Statistics
```bash
perf stat -e cycles,instructions ./myprogram
```
This command displays cycle and instruction counts for `myprogram`.

### Recording Performance Data
```bash
perf record -e cpu-clock ./myprogram
```
It records CPU clock performance data for `myprogram`.

### Reporting Recorded Data
```bash
perf report
```
Generate a report from previously recorded data.

### Listing Events
```bash
perf list
```
This lists all available performance events that `perf` can monitor.

### Real-time Monitoring
```bash
perf top
```
Displays a real-time view of the system performance data.

### Annotating Recorded Data
```bash
perf annotate
```
Shows annotated source code and assembly with performance data for deeper analysis.

## Cheat Sheet

```shell
# Measure program performance
perf stat ./program

# Record performance data
perf record ./program

# Analyze recorded data
perf report

# List all performance events
perf list

# Real-time monitoring
perf top

# Code annotation
perf annotate
```
