```
Slowest: 1024 4096
```

```sh
[hdfs@ip-172-31-5-105 ~]$ ./YARNtest.sh
Testing loop started on Qua Abr 5 11:02:43 UTC 2017
Mapper JVM: 819
Reducer JVM: 819

real    0m51.703s
user    0m6.600s
sys     0m0.291s

real    4m27.811s
user    0m9.611s
sys     0m0.392s
Deleted /results/tg-10GB-8-1-1024
Deleted /results/ts-10GB-8-1-1024
Mapper JVM: 3276
Reducer JVM: 3276

real    0m9.191s
user    0m5.956s
sys     0m0.267s

real    0m2.730s
user    0m3.698s
sys     0m0.187s
Deleted /results/tg-10GB-8-1-4096
rm: `/results/ts-10GB-8-1-4096': No such file or directory
Testing loop ended on Qua Abr 5 11:08:25 UTC 2017
```

```
Fastest: 512 1024
```

```sh
[hdfs@ip-172-31-5-105 ~]$ ./YARNtest.sh
Testing loop started on Qua Abr 5 10:44:58 UTC 2017
Mapper JVM: 409
Reducer JVM: 409

real    0m55.919s
user    0m5.935s
sys     0m0.296s

real    4m10.304s
user    0m8.486s
sys     0m0.381s
Deleted /results/tg-10GB-8-1-512
Deleted /results/ts-10GB-8-1-512
Mapper JVM: 819
Reducer JVM: 819

real    0m51.436s
user    0m5.946s
sys     0m0.265s

real    4m5.137s
user    0m8.519s
sys     0m0.411s
Deleted /results/tg-10GB-8-1-1024
Deleted /results/ts-10GB-8-1-1024
Testing loop ended on Qua Abr 5 10:55:12 UTC 2017
```
