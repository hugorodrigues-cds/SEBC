### Generate data to replication

```sh
su hdfs -c "hadoop jar /opt/cloudera/parcels/CDH-5.10.1-1.cdh5.10.1.p0.10/jars/hadoop-examples.jar teragen 500000 /benchmark/hugorodrigues-cds"
```

### Data replication using distCp beteween me and my partners cluster

```sh
su hdfs -c "hadoop distcp hdfs://ec2-34-207-208-5.compute-1.amazonaws.com:8020/benchmark/hugorodrigues-cds/ hdfs://ec2-52-201-248-69.compute-1.amazonaws.com:8020/benchmark/hugorodrigues-cds/"
```

### Data replicated
```sh
[root@ip-172-31-5-105 ~]# su hdfs -c "hdfs fsck /benchmark/hugorodrigues-cds/ -files -blocks"
Connecting to namenode via http://ip-172-31-5-105.ec2.internal:50070
FSCK started by hdfs (auth:SIMPLE) from /172.31.5.105 for path /benchmark/hugorodrigues-cds/ at Tue Apr 04 15:17:14 UTC 2017
/benchmark/hugorodrigues-cds/ <dir>
/benchmark/hugorodrigues-cds/_SUCCESS 0 bytes, 0 block(s):  OK

/benchmark/hugorodrigues-cds/part-m-00000 25000000 bytes, 1 block(s):  OK
0. BP-1480037614-172.31.5.105-1491312715653:blk_1073742571_1747 len=25000000 Live_repl=3

/benchmark/hugorodrigues-cds/part-m-00001 25000000 bytes, 1 block(s):  OK
0. BP-1480037614-172.31.5.105-1491312715653:blk_1073742572_1748 len=25000000 Live_repl=3

Status: HEALTHY
 Total size:    50000000 B
 Total dirs:    1
 Total files:   3
 Total symlinks:                0
 Total blocks (validated):      2 (avg. block size 25000000 B)
 Minimally replicated blocks:   2 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          4
 Number of racks:               1
FSCK ended at Tue Apr 04 15:17:14 UTC 2017 in 2 milliseconds


The filesystem under path '/benchmark/hugorodrigues-cds/' is HEALTHY
```

