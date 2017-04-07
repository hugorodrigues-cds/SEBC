### The hostname of your db server node

```sh
[root@ip-172-31-11-214 ~]# hostname -f
ip-172-31-11-214.ec2.internal
``´

### The command and output for display your database server's version
```sh
[root@ip-172-31-11-214 ~]# mysql -V
mysql  Ver 15.1 Distrib 10.1.22-MariaDB, for Linux (x86_64) using readline 5.1
```

### The command and output for listing your created databases
```sh
MariaDB [(none)]> show databases;
+--------------------+
| Database           |
+--------------------+
| amon               |
| hue                |
| information_schema |
| metastore          |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
10 rows in set (0.00 sec)
```