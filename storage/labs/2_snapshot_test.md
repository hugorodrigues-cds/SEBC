### Create a precious directory in HDFS; copy the ZIP course file into it.
```sh
[root@ip-172-31-5-105 ~] su hdfs -c "hadoop fs -mkdir /precious"
```
```sh
[hdfs@ip-172-31-5-105 ~] hadoop fs -put SEBC-master.zip /precious
```

### Enable snapshots for precious
```sh
[hdfs@ip-172-31-5-105 ~]$ hdfs dfsadmin -allowSnapshot hdfs://ip-172-31-5-105.ec2.internal:8020/precious
Allowing snaphot on hdfs://ip-172-31-5-105.ec2.internal:8020/precious succeeded
```
### Create a snapshot called sebc-hdfs-test
```sh
[hdfs@ip-172-31-5-105 ~]$ hdfs dfs -createSnapshot hdfs://ip-172-31-5-105.ec2.internal:8020/precious/ sebc-hdfs-test
Created snapshot /precious/.snapshot/sebc-hdfs-test
```
### Delete the directory
```sh

```
### Delete the ZIP file
```sh

```
### Restore the deleted file
```sh

```
### Capture the NameNode web UI screen that lists snapshots in storage/labs/2_snapshot_list.png.
