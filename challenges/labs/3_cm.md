### The command and output for hdfs dfs -ls /user
```sh
[root@ip-172-31-2-90 ~]# su hdfs -c "hdfs dfs -ls /user"
Found 6 items
drwxrwxrwx   - mapred  hadoop              0 2017-04-07 14:04 /user/history
drwxrwxr-t   - hive    hive                0 2017-04-07 14:05 /user/hive
drwxrwxr-x   - hue     hue                 0 2017-04-07 14:05 /user/hue
drwxr-xr-x   - neymar  supergroup          0 2017-04-07 14:09 /user/neymar
drwxrwxr-x   - oozie   oozie               0 2017-04-07 14:06 /user/oozie
drwxr-xr-x   - ronaldo supergroup          0 2017-04-07 14:09 /user/ronaldo
```

### The output from the CM API call ../api/v14/hosts
```sh
[root@ip-172-31-2-90 ~]# curl -u admin:admin 'http://ip-172-31-2-90.ec2.internal:7180/api/v14/hosts'
{
  "items" : [ {
    "hostId" : "86e26928-c81b-4634-9166-9454c9a3a6d0",
    "ipAddress" : "172.31.11.214",
    "hostname" : "ip-172-31-11-214.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-90.ec2.internal:7180/cmf/hostRedirect/86e26928-c81b-4634-9166-9454c9a3a6d0",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "3ace30ee-de85-4957-a985-f6143d3f5c94",
    "ipAddress" : "172.31.2.90",
    "hostname" : "ip-172-31-2-90.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-90.ec2.internal:7180/cmf/hostRedirect/3ace30ee-de85-4957-a985-f6143d3f5c94",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "e6eb22d8-9643-4303-b742-9f77b0e6a49d",
    "ipAddress" : "172.31.3.172",
    "hostname" : "ip-172-31-3-172.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-90.ec2.internal:7180/cmf/hostRedirect/e6eb22d8-9643-4303-b742-9f77b0e6a49d",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "56dfcbd7-9d57-45f4-a8b2-90fc788a6fd6",
    "ipAddress" : "172.31.5.109",
    "hostname" : "ip-172-31-5-109.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-90.ec2.internal:7180/cmf/hostRedirect/56dfcbd7-9d57-45f4-a8b2-90fc788a6fd6",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  } ]
}
```