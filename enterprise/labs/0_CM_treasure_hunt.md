### What is ubertask optimization?
Runs small jobs in sequence in a single JVM 

### Where in CM is the Kerberos Security Realm value displayed?
Administration > Settings > Kerberos
 
### Which CDH service(s) host a property for enabling Kerberos authentication?
* HDFS	Kerberos, SPNEGO (HttpFS)
* MapReduce	Kerberos (also see HDFS)
* YARN	Kerberos (also see HDFS)
* Accumulo	Kerberos (partial)
 *Flume	Kerberos (starting CDH 5.4)
* HBase	Kerberos (HBase Thrift and REST clients must perform their own user authentication)
* HiveServer2	Kerberos, LDAP, Custom/pluggable authentication
* Hive Metastore	Kerberos
* Hue	Kerberos, LDAP, SAML, Custom/pluggable authentication
* Impala	Kerberos, LDAP, SPNEGO (Impala Web Console)
* Oozie	Kerberos, SPNEGO
* Pig	Kerberos
* Search	Kerberos, SPNEGO
* Sentry	Kerberos
* Spark	Kerberos
* Sqoop	Kerberos
* Sqoop2	Kerberos (starting CDH 5.4)
* Zookeeper	Kerberos
* Cloudera Manager	Kerberos, LDAP, SAML
* Cloudera Navigator	See Cloudera Manager
* Backup and Disaster Recovery	See Cloudera Manager

### How do you upgrade the CM agents?
You can use an upgrade wizard that is invoked when you connect to the Admin Console or manually install the Cloudera Manager Agent packages.

### Give the tsquery statement used to chart Hue's CPU utilization?
select cpu_system_rate + cpu_user_rate where category=ROLE and serviceName=$SERVICENAME

### Name all the roles that make up the Hive service

* Hive Metastore Server
* WebHCat Server
* WebHCat Server
* Gateway

### What steps must be completed before integrating Cloudera Manager with Kerberos?
you must configure TLS encryption between Cloudera Manager Server and all cluster hosts with encrypted communications between a Web browser and Cloudera Manager, and between Agents and Cloudera Manager.
You need to have a MIT Kerberos KDC configured.

