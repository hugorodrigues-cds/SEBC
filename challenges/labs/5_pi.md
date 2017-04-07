### Run the Hadoop pi program as the user ronaldo
```sh
[root@ip-172-31-2-90 ~]# kinit ronaldo
Password for ronaldo@HUGORODRIGUES.BR:
[root@ip-172-31-2-90 ~]# hadoop jar /opt/cloudera/parcels/CDH-5.10.1-1.cdh5.10.1.p0.10/jars/hadoop-examples.jar pi 5 1000
Number of Maps  = 5
Samples per Map = 1000
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Starting Job
17/04/07 18:28:18 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-2-90.ec2.internal/172.31.2.90:8032
17/04/07 18:28:18 INFO hdfs.DFSClient: Created token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@HUGORODRIGUES.BR, renewer=yarn, realUser=, issueDate=1491589698241, maxDate=1492194498241, sequenceNumber=11, masterKeyId=2 on ha-hdfs:nameservice1
17/04/07 18:28:18 INFO security.TokenCache: Got dt for hdfs://nameservice1; Kind: HDFS_DELEGATION_TOKEN, Service: ha-hdfs:nameservice1, Ident: (token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@HUGORODRIGUES.BR, renewer=yarn, realUser=, issueDate=1491589698241, maxDate=1492194498241, sequenceNumber=11, masterKeyId=2)
17/04/07 18:28:18 INFO input.FileInputFormat: Total input paths to process : 5
17/04/07 18:28:18 INFO mapreduce.JobSubmitter: number of splits:5
17/04/07 18:28:18 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1491585935317_0010
17/04/07 18:28:18 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: ha-hdfs:nameservice1, Ident: (token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@HUGORODRIGUES.BR, renewer=yarn, realUser=, issueDate=1491589698241, maxDate=1492194498241, sequenceNumber=11, masterKeyId=2)
17/04/07 18:28:19 INFO impl.YarnClientImpl: Submitted application application_1491585935317_0010
17/04/07 18:28:19 INFO mapreduce.Job: The url to track the job: http://ip-172-31-2-90.ec2.internal:8088/proxy/application_1491585935317_0010/
17/04/07 18:28:19 INFO mapreduce.Job: Running job: job_1491585935317_0010
17/04/07 18:28:27 INFO mapreduce.Job: Job job_1491585935317_0010 running in uber mode : false
17/04/07 18:28:27 INFO mapreduce.Job:  map 0% reduce 0%
17/04/07 18:28:35 INFO mapreduce.Job:  map 20% reduce 0%
17/04/07 18:28:38 INFO mapreduce.Job:  map 100% reduce 0%
17/04/07 18:28:45 INFO mapreduce.Job:  map 100% reduce 100%
17/04/07 18:28:45 INFO mapreduce.Job: Job job_1491585935317_0010 completed successfully
17/04/07 18:28:45 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=69
                FILE: Number of bytes written=768706
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=1325
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=23
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=5
                Launched reduce tasks=1
                Data-local map tasks=5
                Total time spent by all maps in occupied slots (ms)=41367
                Total time spent by all reduces in occupied slots (ms)=3551
                Total time spent by all map tasks (ms)=41367
                Total time spent by all reduce tasks (ms)=3551
                Total vcore-seconds taken by all map tasks=41367
                Total vcore-seconds taken by all reduce tasks=3551
                Total megabyte-seconds taken by all map tasks=42359808
                Total megabyte-seconds taken by all reduce tasks=3636224
        Map-Reduce Framework
                Map input records=5
                Map output records=10
                Map output bytes=90
                Map output materialized bytes=170
                Input split bytes=735
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=170
                Reduce input records=10
                Reduce output records=0
                Spilled Records=20
                Shuffled Maps =5
                Failed Shuffles=0
                Merged Map outputs=5
                GC time elapsed (ms)=235
                CPU time spent (ms)=4710
                Physical memory (bytes) snapshot=2509094912
                Virtual memory (bytes) snapshot=9510842368
                Total committed heap usage (bytes)=2843213824
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=590
        File Output Format Counters
                Bytes Written=97
Job Finished in 27.722 seconds
Estimated value of Pi is 3.14160000000000000000
```