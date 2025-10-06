# `hadoop` Command in Linux

The `hadoop` command is used to interface with the Hadoop Framework, which supports the processing of large data sets in a distributed computing environment. This command is a gateway to various Hadoop subcommands and configurations.

## Common Options

| Option          | Description                                                            |
|-----------------|------------------------------------------------------------------------|
| `fs`            | Hadoop file system shell commands.                                     |
| `version`       | Displays the Hadoop version and other related information.             |
| `jar`           | Runs a jar file. The user must specify the file as the first argument. |
| `daemonlog`     | Get/set the log level for each daemon.                                 |
| `namenode`      | Command to start the Hadoop NameNode.                                  |
| `datanode`      | Command to start the Hadoop DataNode.                                  |
| `jobtracker`    | Command to start the JobTracker daemon.                                |
| `tasktracker`   | Command to start the TaskTracker daemon.                               |
| `dfsadmin`      | Hadoop DFS admin commands.                                             |
| `classroom`     | Displays help related to Hadoop classes.                               |

## Usage Examples

### Check Hadoop Version
```bash
hadoop version
```

### List Files in HDFS
```bash
hadoop fs -ls /
```

### Copy a File to HDFS
```bash
hadoop fs -put /local/path/file.txt /hdfs/path/
```

### Run a Jar File
```bash
hadoop jar myapp.jar org.myorg.MyApp input output
```

### Set Log Level for a Daemon
```bash
hadoop daemonlog -setlevel localhost:50070 INFO
```

## Cheat Sheet

```markdown
# Check Hadoop Version
hadoop version

# List files in HDFS
hadoop fs -ls <dir>

# Put a file in HDFS
hadoop fs -put <local> <hdfs>

# Run a .jar file
hadoop jar <jarfile> <mainclass> <args...>

# Manage DFS admin commands
hadoop dfsadmin <command>
```

This guide provides a quick overview and practical usage scenarios for the `hadoop` command to facilitate interaction with Hadoop services and management of file systems.
