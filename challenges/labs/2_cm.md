### Configure the CM repo to install the latest release List the command and output for ls /etc/yum.repos.d

```sh
[root@ip-172-31-2-90 ~]# ls /etc/yum.repos.d
CentOS-Base.repo  CentOS-Debuginfo.repo  CentOS-Media.repo    CentOS-Vault.repo      MariaDB.repo
CentOS-CR.repo    CentOS-fasttrack.repo  CentOS-Sources.repo  cloudera-manager.repo
```

### Configure Cloudera Manager. Use the scm_prepare_database.sh script to write your db.properties file

```sh
[root@ip-172-31-2-90 ~]# /usr/share/cmf/schema/scm_prepare_database.sh mysql -h ip-172-31-11-214.ec2.internal scm scm scm
JAVA_HOME=/usr/java/jdk1.7.0_67-cloudera
Verifying that we can write to /etc/cloudera-scm-server
Creating SCM configuration file in /etc/cloudera-scm-server
Executing:  /usr/java/jdk1.7.0_67-cloudera/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
[                          main] DbCommandExecutor              INFO  Successfully connected to database.
All done, your SCM database is configured correctly!
```