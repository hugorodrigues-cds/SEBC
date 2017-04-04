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
17/04/04 16:37:23 INFO mapreduce.Job:  map 13% reduce 0%
17/04/04 16:37:29 INFO mapreduce.Job:  map 17% reduce 0%
17/04/04 16:37:36 INFO mapreduce.Job:  map 25% reduce 0%
17/04/04 16:37:42 INFO mapreduce.Job:  map 29% reduce 0%
17/04/04 16:37:48 INFO mapreduce.Job:  map 35% reduce 0%
17/04/04 16:37:54 INFO mapreduce.Job:  map 41% reduce 0%
17/04/04 16:38:00 INFO mapreduce.Job:  map 46% reduce 0%
17/04/04 16:38:06 INFO mapreduce.Job:  map 53% reduce 0%
17/04/04 16:38:12 INFO mapreduce.Job:  map 58% reduce 0%
17/04/04 16:38:18 INFO mapreduce.Job:  map 63% reduce 0%
17/04/04 16:38:24 INFO mapreduce.Job:  map 70% reduce 0%
17/04/04 16:38:30 INFO mapreduce.Job:  map 74% reduce 0%
17/04/04 16:38:36 INFO mapreduce.Job:  map 80% reduce 0%
17/04/04 16:38:42 INFO mapreduce.Job:  map 86% reduce 0%
17/04/04 16:38:48 INFO mapreduce.Job:  map 90% reduce 0%
17/04/04 16:38:54 INFO mapreduce.Job:  map 97% reduce 0%
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

