### /etc/cloudera-scm-agent/config.ini

```sh
[root@ip-172-31-11-214 ~]# cat /etc/cloudera-scm-agent/config.ini | grep tls
use_tls=1
[root@ip-172-31-11-214 ~]#
```

### CM Configs

```sh
MariaDB [scm]> select CONFIG_ID, ATTR, VALUE from CONFIGS WHERE CONFIG_ID >=156;
+-----------+--------------------------------+-------------------------------------------------------------+
| CONFIG_ID | ATTR                           | VALUE                                                       |
+-----------+--------------------------------+-------------------------------------------------------------+
|       156 | keystore_password              | 12345678                                                    |
|       157 | keystore_path                  | /opt/cloudera/security/ip-172-31-2-90.ec2.internal.jks      |
|       158 | web_tls                        | true                                                        |
|       159 | ssl_client_truststore_location | /usr/java/jdk1.7.0_67-cloudera/jre/lib/security/jssecacerts |
|       160 | ssl_client_truststore_password | changeit                                                    |
|       161 | agent_tls                      | true                                                        |
+-----------+--------------------------------+-------------------------------------------------------------+
6 rows in set (0.00 sec)
```
