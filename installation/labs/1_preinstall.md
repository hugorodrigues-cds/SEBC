### Check vm.swappiness on all your nodes

```sh 
[root@ip-172-31-5-105 ~]# cat /proc/sys/vm/swappiness
10
```
### Show the mount attributes of your volume(s)


```sh
[root@ip-172-31-5-105 ~]# df -h
Sist. Arq.      Tam. Usado Disp. Uso% Montado em
/dev/xvda1       80G  3,6G   77G   5% /
devtmpfs        7,3G     0  7,3G   0% /dev
tmpfs           7,2G     0  7,2G   0% /dev/shm
tmpfs           7,2G   17M  7,2G   1% /run
tmpfs           7,2G     0  7,2G   0% /sys/fs/cgroup
/dev/xvdb        37G   49M   35G   1% /mnt
tmpfs           1,5G     0  1,5G   0% /run/user/1000
```
### If you have ext-based volumes, list the reserve space setting XFS volumes do not support reserve space

### Disable transparent hugepage support

```sh
[root@ip-172-31-5-105 ~]# cat /boot/grub/grub.conf
default=0
timeout=0


title CentOS Linux (3.10.0-514.10.2.el7.x86_64) 7 (Core)
        root (hd0)
        kernel /boot/vmlinuz-3.10.0-514.10.2.el7.x86_64 ro root=UUID=ef6ba050-6cdc-416a-9380-c14304d0d206 console=hvc0 LANG=en_US.UTF-8 transparent_hugepage=never
        initrd /boot/initramfs-3.10.0-514.10.2.el7.x86_64.img
title CentOS Linux 7 (3.10.0-327.10.1.el7.x86_64)
        root (hd0)
        kernel /boot/vmlinuz-3.10.0-327.10.1.el7.x86_64 ro root=UUID=ef6ba050-6cdc-416a-9380-c14304d0d206 console=hvc0 LANG=en_US.UTF-8 transparent_hugepage=never
        initrd /boot/initramfs-3.10.0-327.10.1.el7.x86_64.img
```

```sh
[root@ip-172-31-5-105 ~]# cat /sys/kernel/mm/transparent_hugepage/enabled
always madvise [never]
```

```sh
[root@ip-172-31-5-105 ~]# cat /sys/kernel/mm/transparent_hugepage/defrag
always madvise [never]
```

### List your network interface configuration

```sh
[root@ip-172-31-5-105 ~]# ip addr
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN qlen 1
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 9001 qdisc pfifo_fast state UP qlen 1000
    link/ether 0a:23:83:37:c2:f2 brd ff:ff:ff:ff:ff:ff
    inet 172.31.5.105/20 brd 172.31.15.255 scope global dynamic eth0
       valid_lft 2262sec preferred_lft 2262sec
    inet6 fe80::823:83ff:fe37:c2f2/64 scope link
       valid_lft forever preferred_lft forever
```

### Show correct forward and reverse host lookups
#### For /etc/hosts, use getent

```sh
[root@ip-172-31-5-105 ~]# getent hosts ec2-54-197-159-209.compute-1.amazonaws.com
172.31.1.146    ec2-54-197-159-209.compute-1.amazonaws.com
```
#### For DNS, use nslookup
```sh
[root@ip-172-31-5-105 ~]# nslookup ec2-54-197-159-209.compute-1.amazonaws
.com
Server:         172.31.0.2
Address:        172.31.0.2#53

Non-authoritative answer:
Name:   ec2-54-197-159-209.compute-1.amazonaws.com
Address: 172.31.1.146
```

### Show the nscd service is running
```sh
[root@ip-172-31-5-105 ~]# systemctl status nscd
                                                                                                                                                                              ● nscd.service - Name Service Cache Daemon
   Loaded: loaded (/usr/lib/systemd/system/nscd.service; enabled; vendor preset: disabled)
   Active: active (running) since Ter 2017-04-04 00:08:38 UTC; 25min ago
  Process: 558 ExecStart=/usr/sbin/nscd $NSCD_OPTIONS (code=exited, status=0/SUCCESS)
 Main PID: 561 (nscd)
   CGroup: /system.slice/nscd.service
           └─561 /usr/sbin/nscd

Abr 04 00:08:38 ip-172-31-5-105.ec2.internal nscd[561]: 561 monitoring directory `/etc` (2)
Abr 04 00:08:38 ip-172-31-5-105.ec2.internal nscd[561]: 561 monitoring file `/etc/services` (6)
Abr 04 00:08:38 ip-172-31-5-105.ec2.internal nscd[561]: 561 monitoring directory `/etc` (2)
Abr 04 00:08:38 ip-172-31-5-105.ec2.internal nscd[561]: 561 disabled inotify-based monitoring for file `/etc/netgroup': No such file or directory
Abr 04 00:08:38 ip-172-31-5-105.ec2.internal nscd[561]: 561 stat failed for file `/etc/netgroup'; will try again later: No such file or directory
Abr 04 00:08:38 ip-172-31-5-105.ec2.internal systemd[1]: Started Name Service Cache Daemon.
Abr 04 00:08:40 ip-172-31-5-105.ec2.internal nscd[561]: 561 monitored file `/etc/resolv.conf` was written to
Abr 04 00:08:40 ip-172-31-5-105.ec2.internal nscd[561]: 561 monitoring file `/etc/resolv.conf` (5)
Abr 04 00:08:40 ip-172-31-5-105.ec2.internal nscd[561]: 561 monitoring directory `/etc` (2)
Abr 04 00:08:57 ip-172-31-5-105.ec2.internal nscd[561]: 561 checking for monitored file `/etc/netgroup': No such file or directory
```
### Show the ntpd service is running
```sh
[root@ip-172-31-5-105 ~]# systemctl status ntpd
● ntpd.service - Network Time Service
   Loaded: loaded (/usr/lib/systemd/system/ntpd.service; enabled; vendor preset: disabled)
   Active: active (running) since Ter 2017-04-04 00:37:31 UTC; 7s ago
  Process: 9259 ExecStart=/usr/sbin/ntpd -u ntp:ntp $OPTIONS (code=exited, status=0/SUCCESS)
 Main PID: 9260 (ntpd)
   CGroup: /system.slice/ntpd.service
           └─9260 /usr/sbin/ntpd -u ntp:ntp -g

Abr 04 00:37:31 ip-172-31-5-105.ec2.internal ntpd[9260]: Listen and drop on 0 v4...
Abr 04 00:37:31 ip-172-31-5-105.ec2.internal ntpd[9260]: Listen and drop on 1 v6...
Abr 04 00:37:31 ip-172-31-5-105.ec2.internal ntpd[9260]: Listen normally on 2 lo...
Abr 04 00:37:31 ip-172-31-5-105.ec2.internal ntpd[9260]: Listen normally on 3 et...
Abr 04 00:37:31 ip-172-31-5-105.ec2.internal ntpd[9260]: Listen normally on 4 lo...
Abr 04 00:37:31 ip-172-31-5-105.ec2.internal ntpd[9260]: Listen normally on 5 et...
Abr 04 00:37:31 ip-172-31-5-105.ec2.internal ntpd[9260]: Listening on routing so...
Abr 04 00:37:31 ip-172-31-5-105.ec2.internal ntpd[9260]: 0.0.0.0 c016 06 restart
Abr 04 00:37:31 ip-172-31-5-105.ec2.internal ntpd[9260]: 0.0.0.0 c012 02 freq_se...
Abr 04 00:37:38 ip-172-31-5-105.ec2.internal ntpd[9260]: 0.0.0.0 c615 05 clock_sync
Hint: Some lines were ellipsized, use -l to show in full.
```
