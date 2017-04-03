### Check vm.swappiness on all your nodes

```sh 
[root@ip-172-31-11-207 ~]# cat /proc/sys/vm/swappiness
10
```
### Show the mount attributes of your volume(s)


```sh
[root@ip-172-31-11-207 ~]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde       7,8G  828M  6,6G  11% /
tmpfs           7,3G     0  7,3G   0% /dev/shm
/dev/xvdf1       37G   48M   37G   1% /data/1
/dev/xvdg1       37G   48M   37G   1% /data/2
```

### Disable transparent hugepage support

```sh
[root@ip-172-31-11-207 ~]# cat /boot/grub/grub.conf
default=0
timeout=1

title CentOS (2.6.32-642.15.1.el6.x86_64)
        root (hd0)
        kernel /boot/vmlinuz-2.6.32-642.15.1.el6.x86_64 root=LABEL=centos_root ro crashkernel=auto LANG=en_US.UTF-8 KEYTABLE=us transparent_hugepage=never
        initrd /boot/initramfs-2.6.32-642.15.1.el6.x86_64.img
title CentOS-6.5-x86_64-GA-03 2.6.32-431.el6.x86_64
        root (hd0)
        kernel /boot/vmlinuz-2.6.32-431.el6.x86_64 root=LABEL=centos_root ro transparent_hugepage=never
        initrd /boot/initramfs-2.6.32-431.el6.x86_64.img
```

### List your network interface configuration

```sh
[root@ip-172-31-11-207 ~]# ip addr
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 9001 qdisc pfifo_fast state UP qlen 1000
    link/ether 0a:b5:ab:db:69:86 brd ff:ff:ff:ff:ff:ff
    inet 172.31.11.207/20 brd 172.31.15.255 scope global eth0
    inet6 fe80::8b5:abff:fedb:6986/64 scope link
       valid_lft forever preferred_lft forever
```

Show correct forward and reverse host lookups
For /etc/hosts, use getent
For DNS, use nslookup
Show the nscd service is running
Show the ntpd service is running
