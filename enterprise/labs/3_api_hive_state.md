### Hive stop (API v14)
```sh
[root@ip-172-31-5-105 ~]# curl -u hugorodrigues-cds:cloudera -X POST 'http://ip-172-31-5-105.ec2.internal:7180/api/v14/clusters/hugorodrigues-cds/services/hive/commands/stop'
{
  "id" : 433,
  "name" : "Stop",
  "startTime" : "2017-04-05T14:39:26.317Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

### Start Hive (API v14)
```sh
[root@ip-172-31-5-105 ~]# curl -u hugorodrigues-cds:cloudera -X POST 'http://ip-172-31-5-105.ec2.internal:7180/api/v14/lusters/hugorodrigues-cds/services/hive/commands/start'
{
  "id" : 437,
  "name" : "Start",
  "startTime" : "2017-04-05T14:44:20.431Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

### Chek Hive (API v14)

```sh
curl -u hugorodrigues-cds:cloudera -X POST 'http://ip-172-31-5-105.ec2.internal:7180/api/v14/clusters/hugorodrigues-cds/services/hive'
```
