```sh
[root@ip-172-31-4-152 ~]# beeline
Beeline version 1.1.0-cdh5.10.1 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-4-152.ec2.internal@EC2.INTERNAL
scan complete in 2ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-4-152.ec2.internal@EC2.INTERNAL
Connected to: Apache Hive (version 1.1.0-cdh5.10.1)
Driver: Hive JDBC (version 1.1.0-cdh5.10.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170406230202_cbb3d267-8420-4832-a7a2-ad2c01cafacc): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170406230202_cbb3d267-8420-4832-a7a2-ad2c01cafacc); Time taken: 0.082 seconds
INFO  : Executing command(queryId=hive_20170406230202_cbb3d267-8420-4832-a7a2-ad2c01cafacc): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170406230202_cbb3d267-8420-4832-a7a2-ad2c01cafacc); Time taken: 0.158 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (0.336 seconds)
```
