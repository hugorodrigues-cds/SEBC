### List the cloud provider you are using (AWS, GCE, Azure, other)
* AWS INSTANCES

### List the nodes you are using by IP address and name
* PUBLIC DNS	PUBLIC IP	HOSTNAME	IP LOCAL
* ec2-54-172-43-228.compute-1.amazonaws.com	54.172.43.228	ip-172-31-11-214.ec2.internal	172.31.11.214
* ec2-107-20-117-254.compute-1.amazonaws.com	107.20.117.254	ip-172-31-2-90.ec2.internal	172.31.2.90
* ec2-54-146-249-95.compute-1.amazonaws.com	54.146.249.95	ip-172-31-3-172.ec2.internal	172.31.3.172
* ec2-34-204-44-131.compute-1.amazonaws.com	34.204.44.131	ip-172-31-5-109.ec2.internal	172.31.5.109

### List the Linux release you are using
```sh
[root@ip-172-31-5-109 ~]# cat /etc/centos-release
CentOS Linux release 7.3.1611 (Core)
```

### Demonstrate the disk capacity available on each node is >= 30 GB
```sh
[root@ip-172-31-5-109 ~]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       60G  1.8G   59G   3% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   25M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
/dev/xvdb        37G   49M   35G   1% /mnt
tmpfs           1.5G     0  1.5G   0% /run/user/0
```
### List the command and output for yum repolist enabled

```sh
root@ip-172-31-5-109 ~]# yum repolist enabled
Loaded plugins: fastestmirror
cloudera-manager                                                                                                                            |  951 B  00:00:00
mariadb                                                                                                                                     | 2.9 kB  00:00:00
mariadb/primary_db                                                                                                                          |  18 kB  00:00:00
cloudera-manager/primary                                                                                                                    | 4.3 kB  00:00:00
Loading mirror speeds from cached hostfile
 * base: repo1.ash.innoscale.net
 * extras: mirror.solarvps.com
 * updates: mirror.symnds.com
cloudera-manager                                                                                                                                               7/7
repo id                                                                      repo name                                                                       status
base/7/x86_64                                                                CentOS-7 - Base                                                                 9,363
cloudera-manager                                                             Cloudera Manager                                                                    7
extras/7/x86_64                                                              CentOS-7 - Extras                                                                 311
mariadb                                                                      MariaDB                                                                            15
updates/7/x86_64                                                             CentOS-7 - Updates                                                              1,126
repolist: 10,822
```
