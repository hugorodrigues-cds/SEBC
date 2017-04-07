###  Run the terasort program as neymar using the output target /user/neymar/tsort640m

```sh
[root@ip-172-31-2-90 ~]# kinit neymar
Password for neymar@HUGORODRIGUES.BR:
[root@ip-172-31-2-90 ~]# hadoop jar /opt/cloudera/parcels/CDH-5.10.1-1.cdh5.10.1.p0.10/jars/hadoop-examples.jar terasort -D mapred.maps.tasks=4 /user/neymar/tgen640 /user/neymar/tsort640m
17/04/07 18:11:21 INFO terasort.TeraSort: starting
17/04/07 18:11:23 INFO hdfs.DFSClient: Created token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@HUGORODRIGUES.BR, renewer=yarn, realUser=, issueDate=1491588683018, maxDate=1492193483018, sequenceNumber=10, masterKeyId=2 on ha-hdfs:nameservice1
17/04/07 18:11:23 INFO security.TokenCache: Got dt for hdfs://nameservice1; Kind: HDFS_DELEGATION_TOKEN, Service: ha-hdfs:nameservice1, Ident: (token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@HUGORODRIGUES.BR, renewer=yarn, realUser=, issueDate=1491588683018, maxDate=1492193483018, sequenceNumber=10, masterKeyId=2)
17/04/07 18:11:23 INFO input.FileInputFormat: Total input paths to process : 8
Spent 391ms computing base-splits.
Spent 6ms computing TeraScheduler splits.
Computing input splits took 399ms
Sampling 10 splits of 392
Making 6 from 100000 sampled records
Computing parititions took 783ms
Spent 1184ms computing partitions.
17/04/07 18:11:24 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-2-90.ec2.internal/172.31.2.90:8032
17/04/07 18:11:24 INFO mapreduce.JobSubmitter: number of splits:392
17/04/07 18:11:24 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1491585935317_0009
17/04/07 18:11:24 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: ha-hdfs:nameservice1, Ident: (token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@HUGORODRIGUES.BR, renewer=yarn, realUser=, issueDate=1491588683018, maxDate=1492193483018, sequenceNumber=10, masterKeyId=2)
17/04/07 18:11:25 INFO impl.YarnClientImpl: Submitted application application_1491585935317_0009
17/04/07 18:11:25 INFO mapreduce.Job: The url to track the job: http://ip-172-31-2-90.ec2.internal:8088/proxy/application_1491585935317_0009/
17/04/07 18:11:25 INFO mapreduce.Job: Running job: job_1491585935317_0009
17/04/07 18:11:33 INFO mapreduce.Job: Job job_1491585935317_0009 running in uber mode : false
17/04/07 18:11:33 INFO mapreduce.Job:  map 0% reduce 0%
17/04/07 18:11:45 INFO mapreduce.Job:  map 1% reduce 0%
17/04/07 18:11:49 INFO mapreduce.Job:  map 2% reduce 0%
17/04/07 18:11:58 INFO mapreduce.Job:  map 3% reduce 0%
17/04/07 18:12:05 INFO mapreduce.Job:  map 4% reduce 0%
17/04/07 18:12:09 INFO mapreduce.Job:  map 5% reduce 0%
17/04/07 18:12:19 INFO mapreduce.Job:  map 6% reduce 0%
17/04/07 18:12:21 INFO mapreduce.Job:  map 7% reduce 0%
17/04/07 18:12:33 INFO mapreduce.Job:  map 8% reduce 0%
17/04/07 18:12:34 INFO mapreduce.Job:  map 9% reduce 0%
17/04/07 18:12:48 INFO mapreduce.Job:  map 11% reduce 0%
17/04/07 18:13:03 INFO mapreduce.Job:  map 13% reduce 0%
17/04/07 18:13:16 INFO mapreduce.Job:  map 14% reduce 0%
17/04/07 18:13:17 INFO mapreduce.Job:  map 15% reduce 0%
17/04/07 18:13:27 INFO mapreduce.Job:  map 16% reduce 0%
17/04/07 18:13:31 INFO mapreduce.Job:  map 17% reduce 0%
17/04/07 18:13:38 INFO mapreduce.Job:  map 18% reduce 0%
17/04/07 18:13:46 INFO mapreduce.Job:  map 19% reduce 0%
17/04/07 18:13:50 INFO mapreduce.Job:  map 20% reduce 0%
17/04/07 18:14:01 INFO mapreduce.Job:  map 21% reduce 0%
17/04/07 18:14:02 INFO mapreduce.Job:  map 22% reduce 0%
17/04/07 18:14:14 INFO mapreduce.Job:  map 23% reduce 0%
17/04/07 18:14:17 INFO mapreduce.Job:  map 24% reduce 0%
17/04/07 18:14:28 INFO mapreduce.Job:  map 25% reduce 0%
17/04/07 18:14:30 INFO mapreduce.Job:  map 26% reduce 0%
17/04/07 18:14:34 INFO mapreduce.Job:  map 27% reduce 0%
17/04/07 18:14:45 INFO mapreduce.Job:  map 29% reduce 0%
17/04/07 18:14:57 INFO mapreduce.Job:  map 30% reduce 0%
17/04/07 18:15:01 INFO mapreduce.Job:  map 31% reduce 0%
17/04/07 18:15:11 INFO mapreduce.Job:  map 32% reduce 0%
17/04/07 18:15:16 INFO mapreduce.Job:  map 33% reduce 0%
17/04/07 18:15:25 INFO mapreduce.Job:  map 34% reduce 0%
17/04/07 18:15:30 INFO mapreduce.Job:  map 35% reduce 0%
17/04/07 18:15:39 INFO mapreduce.Job:  map 36% reduce 0%
17/04/07 18:15:45 INFO mapreduce.Job:  map 37% reduce 0%
17/04/07 18:15:52 INFO mapreduce.Job:  map 38% reduce 0%
17/04/07 18:15:53 INFO mapreduce.Job:  map 39% reduce 0%
17/04/07 18:16:03 INFO mapreduce.Job:  map 40% reduce 0%
17/04/07 18:16:08 INFO mapreduce.Job:  map 41% reduce 0%
17/04/07 18:16:16 INFO mapreduce.Job:  map 42% reduce 0%
17/04/07 18:16:23 INFO mapreduce.Job:  map 43% reduce 0%
17/04/07 18:16:30 INFO mapreduce.Job:  map 44% reduce 0%
17/04/07 18:16:38 INFO mapreduce.Job:  map 45% reduce 0%
17/04/07 18:16:44 INFO mapreduce.Job:  map 46% reduce 0%
17/04/07 18:16:53 INFO mapreduce.Job:  map 47% reduce 0%
17/04/07 18:16:59 INFO mapreduce.Job:  map 48% reduce 0%
17/04/07 18:17:07 INFO mapreduce.Job:  map 49% reduce 0%
17/04/07 18:17:11 INFO mapreduce.Job:  map 50% reduce 0%
17/04/07 18:17:15 INFO mapreduce.Job:  map 51% reduce 0%
17/04/07 18:17:22 INFO mapreduce.Job:  map 52% reduce 0%
17/04/07 18:17:30 INFO mapreduce.Job:  map 53% reduce 0%
17/04/07 18:17:37 INFO mapreduce.Job:  map 54% reduce 0%
17/04/07 18:17:45 INFO mapreduce.Job:  map 55% reduce 0%
17/04/07 18:17:51 INFO mapreduce.Job:  map 56% reduce 0%
17/04/07 18:17:59 INFO mapreduce.Job:  map 57% reduce 0%
17/04/07 18:18:06 INFO mapreduce.Job:  map 58% reduce 0%
17/04/07 18:18:14 INFO mapreduce.Job:  map 59% reduce 0%
17/04/07 18:18:18 INFO mapreduce.Job:  map 60% reduce 0%
17/04/07 18:18:28 INFO mapreduce.Job:  map 61% reduce 0%
17/04/07 18:18:29 INFO mapreduce.Job:  map 62% reduce 0%
17/04/07 18:18:35 INFO mapreduce.Job:  map 63% reduce 0%
17/04/07 18:18:42 INFO mapreduce.Job:  map 64% reduce 0%
17/04/07 18:18:48 INFO mapreduce.Job:  map 65% reduce 0%
17/04/07 18:18:56 INFO mapreduce.Job:  map 66% reduce 0%
17/04/07 18:19:03 INFO mapreduce.Job:  map 67% reduce 0%
17/04/07 18:19:10 INFO mapreduce.Job:  map 68% reduce 0%
17/04/07 18:19:17 INFO mapreduce.Job:  map 69% reduce 0%
17/04/07 18:19:25 INFO mapreduce.Job:  map 70% reduce 0%
17/04/07 18:19:33 INFO mapreduce.Job:  map 71% reduce 0%
17/04/07 18:19:36 INFO mapreduce.Job:  map 72% reduce 0%
17/04/07 18:19:46 INFO mapreduce.Job:  map 73% reduce 0%
17/04/07 18:19:49 INFO mapreduce.Job:  map 74% reduce 0%
17/04/07 18:19:58 INFO mapreduce.Job:  map 75% reduce 0%
17/04/07 18:20:03 INFO mapreduce.Job:  map 76% reduce 0%
17/04/07 18:20:09 INFO mapreduce.Job:  map 77% reduce 0%
17/04/07 18:20:18 INFO mapreduce.Job:  map 78% reduce 0%
17/04/07 18:20:24 INFO mapreduce.Job:  map 79% reduce 0%
17/04/07 18:20:31 INFO mapreduce.Job:  map 80% reduce 0%
17/04/07 18:20:38 INFO mapreduce.Job:  map 81% reduce 0%
17/04/07 18:20:42 INFO mapreduce.Job:  map 82% reduce 0%
17/04/07 18:20:50 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000000_0, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#9
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:20:50 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000001_0, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#1
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:20:51 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000002_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_0 from host ip-172-31-3-172.ec2.internal
17/04/07 18:20:51 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000003_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_0 from host ip-172-31-3-172.ec2.internal
17/04/07 18:20:51 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000002_0, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#10
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:20:57 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000004_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:57 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000006_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:57 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000005_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:57 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000021_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:57 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000041_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:57 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000014_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:57 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000022_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:57 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000013_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:57 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000007_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:57 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000040_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:58 INFO mapreduce.Job:  map 76% reduce 0%
17/04/07 18:20:58 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000015_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:58 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000039_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:58 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000031_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:58 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000023_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:58 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000030_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:58 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000029_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:58 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000001_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:58 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000004_0, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#8
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:20:58 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000028_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:58 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000026_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:59 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000020_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:59 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000027_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:59 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000018_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:59 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000011_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:59 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000019_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:59 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000010_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:59 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000012_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:59 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000036_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_0 from host ip-172-31-5-109.ec2.internal
17/04/07 18:20:59 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000003_0, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#1
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:21:06 INFO mapreduce.Job:  map 77% reduce 0%
17/04/07 18:21:13 INFO mapreduce.Job:  map 78% reduce 0%
17/04/07 18:21:22 INFO mapreduce.Job:  map 79% reduce 0%
17/04/07 18:21:26 INFO mapreduce.Job:  map 80% reduce 0%
17/04/07 18:21:36 INFO mapreduce.Job:  map 81% reduce 0%
17/04/07 18:21:37 INFO mapreduce.Job:  map 82% reduce 0%
17/04/07 18:21:47 INFO mapreduce.Job:  map 83% reduce 0%
17/04/07 18:21:51 INFO mapreduce.Job:  map 84% reduce 0%
17/04/07 18:21:52 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000038_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:52 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000037_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:52 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000035_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:52 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000008_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:52 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000034_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:52 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000009_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:52 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000033_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:52 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000016_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:52 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000032_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:52 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000025_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:53 INFO mapreduce.Job:  map 80% reduce 0%
17/04/07 18:21:53 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000017_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:53 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000000_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:53 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000024_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_1 from host ip-172-31-5-109.ec2.internal
17/04/07 18:21:53 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000002_1, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#8
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:21:54 INFO mapreduce.Job:  map 81% reduce 0%
17/04/07 18:21:56 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000047_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000000_1 from host ip-172-31-3-172.ec2.internal
17/04/07 18:21:56 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000044_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000000_1 from host ip-172-31-3-172.ec2.internal
17/04/07 18:21:56 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000045_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000000_1 from host ip-172-31-3-172.ec2.internal
17/04/07 18:21:56 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000048_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000000_1 from host ip-172-31-3-172.ec2.internal
17/04/07 18:21:56 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000049_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000000_1 from host ip-172-31-3-172.ec2.internal
17/04/07 18:21:56 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000046_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000000_1 from host ip-172-31-3-172.ec2.internal
17/04/07 18:21:56 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000043_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000000_1 from host ip-172-31-3-172.ec2.internal
17/04/07 18:21:56 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000000_1, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#10
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:21:56 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000001_1, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#10
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:21:57 INFO mapreduce.Job:  map 79% reduce 0%
17/04/07 18:22:02 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000042_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:02 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000066_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:02 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000067_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:02 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000065_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:02 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000057_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:02 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000055_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:02 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000056_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:02 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000004_1, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#10
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:22:02 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000051_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:02 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000053_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:03 INFO mapreduce.Job:  map 74% reduce 0%
17/04/07 18:22:03 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000074_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:03 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000091_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:03 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000092_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:03 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000082_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:04 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000073_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:04 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000070_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:04 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000083_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:04 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000093_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:04 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000079_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_1 from host ip-172-31-11-214.ec2.internal
17/04/07 18:22:04 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000003_1, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#9
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:22:05 INFO mapreduce.Job:  map 75% reduce 0%
17/04/07 18:22:07 INFO mapreduce.Job:  map 76% reduce 0%
17/04/07 18:22:18 INFO mapreduce.Job:  map 77% reduce 0%
17/04/07 18:22:22 INFO mapreduce.Job:  map 78% reduce 0%
17/04/07 18:22:31 INFO mapreduce.Job:  map 79% reduce 0%
17/04/07 18:22:37 INFO mapreduce.Job:  map 80% reduce 0%
17/04/07 18:22:41 INFO mapreduce.Job:  map 81% reduce 0%
17/04/07 18:22:50 INFO mapreduce.Job:  map 82% reduce 0%
17/04/07 18:22:52 INFO mapreduce.Job:  map 83% reduce 0%
17/04/07 18:23:03 INFO mapreduce.Job:  map 84% reduce 0%
17/04/07 18:23:06 INFO mapreduce.Job:  map 85% reduce 0%
17/04/07 18:23:13 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000099_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000001_2 from host ip-172-31-3-172.ec2.internal
17/04/07 18:23:13 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000101_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000001_2 from host ip-172-31-3-172.ec2.internal
17/04/07 18:23:13 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000001_2, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#3
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:23:14 INFO mapreduce.Job:  map 84% reduce 0%
17/04/07 18:23:16 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000050_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_2 from host ip-172-31-11-214.ec2.internal
17/04/07 18:23:16 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000100_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_2 from host ip-172-31-11-214.ec2.internal
17/04/07 18:23:16 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000054_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_2 from host ip-172-31-11-214.ec2.internal
17/04/07 18:23:16 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000052_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_2 from host ip-172-31-11-214.ec2.internal
17/04/07 18:23:16 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000064_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_2 from host ip-172-31-11-214.ec2.internal
17/04/07 18:23:16 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000062_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000003_2 from host ip-172-31-11-214.ec2.internal
17/04/07 18:23:16 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000003_2, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#10
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:23:16 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000108_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:16 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000109_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:16 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000107_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:17 INFO mapreduce.Job:  map 77% reduce 0%
17/04/07 18:23:17 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000078_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:17 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000072_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:17 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000096_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:17 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000071_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:17 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000106_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:17 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000080_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:17 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000086_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:17 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000105_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:17 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000087_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:17 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000075_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:18 INFO mapreduce.Job:  map 78% reduce 0%
17/04/07 18:23:18 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000063_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:18 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000098_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:18 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000081_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:18 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000088_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:18 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000097_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000004_2 from host ip-172-31-5-109.ec2.internal
17/04/07 18:23:18 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000004_2, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#1
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:23:18 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000119_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_2 from host ip-172-31-11-214.ec2.internal
17/04/07 18:23:18 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000118_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_2 from host ip-172-31-11-214.ec2.internal
17/04/07 18:23:18 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000104_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000002_2 from host ip-172-31-11-214.ec2.internal
17/04/07 18:23:18 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000002_2, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#1
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:23:25 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_r_000000_2, Status : FAILED
Error: org.apache.hadoop.mapreduce.task.reduce.Shuffle$ShuffleError: error in shuffle in fetcher#10
        at org.apache.hadoop.mapreduce.task.reduce.Shuffle.run(Shuffle.java:134)
        at org.apache.hadoop.mapred.ReduceTask.run(ReduceTask.java:376)
        at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Exceeded MAX_FAILED_UNIQUE_FETCHES; bailing-out.
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.checkReducerHealth(ShuffleSchedulerImpl.java:391)
        at org.apache.hadoop.mapreduce.task.reduce.ShuffleSchedulerImpl.copyFailed(ShuffleSchedulerImpl.java:306)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.copyFromHost(Fetcher.java:366)
        at org.apache.hadoop.mapreduce.task.reduce.Fetcher.run(Fetcher.java:198)

17/04/07 18:23:30 INFO mapreduce.Job:  map 79% reduce 0%
17/04/07 18:23:32 INFO mapreduce.Job:  map 80% reduce 0%
17/04/07 18:23:40 INFO mapreduce.Job:  map 81% reduce 0%
17/04/07 18:23:46 INFO mapreduce.Job:  map 82% reduce 0%
17/04/07 18:23:51 INFO mapreduce.Job:  map 83% reduce 0%
17/04/07 18:24:01 INFO mapreduce.Job:  map 84% reduce 0%
17/04/07 18:24:02 INFO mapreduce.Job:  map 85% reduce 0%
17/04/07 18:24:12 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000117_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000001_3 from host ip-172-31-11-214.ec2.internal
17/04/07 18:24:12 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000126_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000001_3 from host ip-172-31-11-214.ec2.internal
17/04/07 18:24:12 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000125_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000001_3 from host ip-172-31-11-214.ec2.internal
17/04/07 18:24:12 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000127_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000001_3 from host ip-172-31-11-214.ec2.internal
17/04/07 18:24:12 INFO mapreduce.Job: Task Id : attempt_1491585935317_0009_m_000059_0, Status : FAILED
Too many fetch failures. Failing the attempt. Last failure reported by attempt_1491585935317_0009_r_000001_3 from host ip-172-31-11-214.ec2.internal
17/04/07 18:24:13 INFO mapreduce.Job:  map 100% reduce 100%
17/04/07 18:24:14 INFO mapreduce.Job: Job job_1491585935317_0009 failed with state FAILED due to: Task failed task_1491585935317_0009_r_000001
Job failed as tasks failed. failedMaps:0 failedReduces:1

17/04/07 18:24:15 INFO mapreduce.Job: Counters: 41
        File System Counters
                FILE: Number of bytes read=18095
                FILE: Number of bytes written=2437057558
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=5519742793
                HDFS: Number of bytes written=0
                HDFS: Number of read operations=987
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=0
        Job Counters
                Failed map tasks=101
                Failed reduce tasks=16
                Killed map tasks=63
                Killed reduce tasks=5
                Launched map tasks=434
                Launched reduce tasks=18
                Other local map tasks=96
                Data-local map tasks=338
                Total time spent by all maps in occupied slots (ms)=5352382
                Total time spent by all reduces in occupied slots (ms)=191210
                Total time spent by all map tasks (ms)=5352382
                Total time spent by all reduce tasks (ms)=191210
                Total vcore-seconds taken by all map tasks=5352382
                Total vcore-seconds taken by all reduce tasks=191210
                Total megabyte-seconds taken by all map tasks=5480839168
                Total megabyte-seconds taken by all reduce tasks=195799040
        Map-Reduce Framework
                Map input records=55197043
                Map output records=55197043
                Map output bytes=5630098386
                Map output materialized bytes=2394597870
                Input split bytes=38493
                Combine input records=0
                Spilled Records=55197043
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=34760
                CPU time spent (ms)=1029470
                Physical memory (bytes) snapshot=154348711936
                Virtual memory (bytes) snapshot=519963234304
                Total committed heap usage (bytes)=183875141632
        File Input Format Counters
                Bytes Read=5519704300
17/04/07 18:24:15 INFO terasort.TeraSort: done

```
