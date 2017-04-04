### teragen
```sh
[root@ip-172-31-5-105 ~]# time su hdfs -c "hadoop jar /opt/cloudera/parcels/CDH-5.10.1-1.cdh5.10.1.p0.10/jars/hadoop-examples.jar teragen 100000000 /benchmark/datagen/data-10GB"
17/04/04 16:36:56 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-5-105.ec2.internal/172.31.5.105:8032
17/04/04 16:36:56 INFO terasort.TeraGen: Generating 100000000 using 2
17/04/04 16:36:56 INFO mapreduce.JobSubmitter: number of splits:2
17/04/04 16:36:57 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1491323117336_0001
17/04/04 16:36:57 INFO impl.YarnClientImpl: Submitted application application_1491323117336_0001
17/04/04 16:36:57 INFO mapreduce.Job: The url to track the job: http://ip-172-31-5-105.ec2.internal:8088/proxy/application_1491323117336_0001/
17/04/04 16:36:57 INFO mapreduce.Job: Running job: job_1491323117336_0001
17/04/04 16:37:04 INFO mapreduce.Job: Job job_1491323117336_0001 running in uber mode : false
17/04/04 16:37:04 INFO mapreduce.Job:  map 0% reduce 0%
17/04/04 16:39:00 INFO mapreduce.Job:  map 100% reduce 0%
17/04/04 16:39:01 INFO mapreduce.Job: Job job_1491323117336_0001 completed successfully
17/04/04 16:39:01 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=249692
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=170
                HDFS: Number of bytes written=10000000000
                HDFS: Number of read operations=8
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=4
        Job Counters
                Launched map tasks=2
                Other local map tasks=2
                Total time spent by all maps in occupied slots (ms)=222872
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=222872
                Total vcore-seconds taken by all map tasks=222872
                Total megabyte-seconds taken by all map tasks=228220928
        Map-Reduce Framework
                Map input records=100000000
                Map output records=100000000
                Input split bytes=170
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1366
                CPU time spent (ms)=147580
                Physical memory (bytes) snapshot=371519488
                Virtual memory (bytes) snapshot=3169423360
                Total committed heap usage (bytes)=434110464
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=214760662691937609
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=10000000000

real    2m8.156s
user    0m6.596s
sys     0m0.275s
```
### terasort
```sh
[root@ip-172-31-5-105 ~]# time su hdfs -c "hadoop jar /opt/cloudera/parcels/CDH-5.10.1-1.cdh5.10.1.p0.10/jars/hadoop-examples.jar terasort -D mapred.maps.tasks=4 /benchmark/datagen/data-10GB /user/hugorodrigues-cds/terasort-result"
17/04/04 16:54:41 INFO terasort.TeraSort: starting
17/04/04 16:54:42 INFO input.FileInputFormat: Total input paths to process : 2
Spent 305ms computing base-splits.
Spent 7ms computing TeraScheduler splits.
Computing input splits took 313ms
Sampling 10 splits of 298
Making 8 from 100000 sampled records
Computing parititions took 880ms
Spent 1195ms computing partitions.
17/04/04 16:54:43 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-5-105.ec2.internal/172.31.5.105:8032
17/04/04 16:54:44 INFO mapreduce.JobSubmitter: number of splits:298
17/04/04 16:54:44 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1491323117336_0002
17/04/04 16:54:44 INFO impl.YarnClientImpl: Submitted application application_1491323117336_0002
17/04/04 16:54:44 INFO mapreduce.Job: The url to track the job: http://ip-172-31-5-105.ec2.internal:8088/proxy/application_1491323117336_0002/
17/04/04 16:54:44 INFO mapreduce.Job: Running job: job_1491323117336_0002
17/04/04 16:54:51 INFO mapreduce.Job: Job job_1491323117336_0002 running in uber mode : false
17/04/04 16:54:51 INFO mapreduce.Job:  map 0% reduce 0%
17/04/04 17:00:20 INFO mapreduce.Job:  map 100% reduce 100%
17/04/04 17:00:21 INFO mapreduce.Job: Job job_1491323117336_0002 completed successfully
17/04/04 17:00:21 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=4441210055
                FILE: Number of bytes written=8822570660
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=10000043508
                HDFS: Number of bytes written=10000000000
                HDFS: Number of read operations=918
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=298
                Launched reduce tasks=8
                Data-local map tasks=298
                Total time spent by all maps in occupied slots (ms)=2533455
                Total time spent by all reduces in occupied slots (ms)=801818
                Total time spent by all map tasks (ms)=2533455
                Total time spent by all reduce tasks (ms)=801818
                Total vcore-seconds taken by all map tasks=2533455
                Total vcore-seconds taken by all reduce tasks=801818
                Total megabyte-seconds taken by all map tasks=2594257920
                Total megabyte-seconds taken by all reduce tasks=821061632
        Map-Reduce Framework
                Map input records=100000000
                Map output records=100000000
                Map output bytes=10200000000
                Map output materialized bytes=4342651795
                Input split bytes=43508
                Combine input records=0
                Combine output records=0
                Reduce input groups=100000000
                Reduce shuffle bytes=4342651795
                Reduce input records=100000000
                Reduce output records=100000000
                Spilled Records=200000000
                Shuffled Maps =2384
                Failed Shuffles=0
                Merged Map outputs=2384
                GC time elapsed (ms)=40835
                CPU time spent (ms)=1490030
                Physical memory (bytes) snapshot=152955494400
                Virtual memory (bytes) snapshot=483366330368
                Total committed heap usage (bytes)=171872092160
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=10000000000
        File Output Format Counters
                Bytes Written=10000000000
17/04/04 17:00:21 INFO terasort.TeraSort: done

real    5m41.269s
user    0m9.926s
sys     0m0.435s
```
