# Practical 2: Hadoop Installation, Configuration and HDFS Operations

## Challenges Faced

1. Configuring Hadoop correctly in a single-node environment.
2. Understanding and remembering HDFS commands for file and directory operations.
3. Configuring Hadoop XML files (`core-site.xml`, `hdfs-site.xml`, `mapred-site.xml`, and `yarn-site.xml`) correctly.
4. Starting Hadoop services and verifying that NameNode, DataNode, SecondaryNameNode, and other Hadoop processes were running using the `jps` command.

## Solutions

1. Followed the Hadoop installation steps carefully, verified all environment variables, and restarted Hadoop services after configuration changes.
2. Practiced HDFS commands (`mkdir`, `put`, `ls`, `cat`, `cp`, `mv`, `get`, `rm`) multiple times to become familiar with their usage.
3. Edited each XML configuration file carefully, checked for syntax errors, and verified the configuration before starting Hadoop services.
4. Used the `jps` command to confirm that all required Hadoop daemons were running and used `hdfs dfsadmin -report` and `hdfs fsck` to verify cluster health and HDFS functionality.
