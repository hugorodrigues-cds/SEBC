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
[hdfs@ip-172-31-5-105 ~]$ hadoop fs -rmr /precious
rmr: Failed to move to trash: hdfs://ip-172-31-5-105.ec2.internal:8020/precious: The directory /precious cannot be deleted since /precious is snapshottable and already has snapshots
```
### Delete the ZIP file
```sh
[hdfs@ip-172-31-5-105 ~]$ hadoop fs -rm /precious/SEBC-master.zip
17/04/04 20:05:41 INFO fs.TrashPolicyDefault: Moved: 'hdfs://ip-172-31-5-105.ec2.internal:8020/precious/SEBC-master.zip' to trash at: hdfs://ip-172-31-5-105.ec2.internal:8020/user/hdfs/.Trash/Current/precious/SEBC-master.zip
```
### Restore the deleted file
```sh
hadoop fs -cp /precious/.snapshot/sebc-hdfs-test/SEBC-master.zip /precious/SEBC-master.zip
```
### Capture the NameNode web UI screen that lists snapshots in storage/labs/2_snapshot_list.png.
