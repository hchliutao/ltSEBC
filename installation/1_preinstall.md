[root@nn01 /]# cat /etc/sysctl.conf | grep vm.swappiness
vm.swappiness = 1
[root@nn01 /]# 

[root@nn01 /]# service ntpd status
ntpd (pid  1909) is running...
[root@nn01 /]# 

[root@nn01 /]# cat /etc/sysconfig/network
NETWORKING=yes
HOSTNAME=nn01
NETWORKING_IPV6=no
NETMASK=255.255.255.0
GATEWAY=192.168.60.254
DNS1=202.102.152.3

[root@nn01 /]# cat /etc/hosts
192.168.60.71 nn01
192.168.60.72 nn02
192.168.60.73 dn01
192.168.60.74 dn02
192.168.60.75 dn03

[root@nn01 /]# service iptables status
iptables: Firewall is not running.
[root@nn01 /]# 

[root@nn01 /]# cat /etc/selinux/config  | grep SELINUX
# SELINUX= can take one of these three values:
#SELINUX=enforcing
SELINUX=disabled

[root@nn01 /]# cd /var/www/html/java/
[root@nn01 java]# pwd
/var/www/html/java

[root@nn01 java]# ll
total 258496
-rw-r--r-- 1 root root 122656363 May 14 21:14 jdk-7u55-linux-x64.rpm
-rw-r--r-- 1 root root 142039186 May 14 21:14 oracle-j2sdk1.7-1.7.0 update67-1.x86_64.rpm
[root@nn01 java]# rpm -ivh jdk-7u55-linux-x64.rpm
[root@nn01 java]#rpm -ivh oracle-j2sdk1.7-1.7.0 update67-1.x86_64.rpm

[root@nn01 /]# java -version
java version "1.7.0_55"
Java(TM) SE Runtime Environment (build 1.7.0_55-b13)
Java HotSpot(TM) 64-Bit Server VM (build 24.55-b03, mixed mode)
[root@nn01 /]# 

[root@nn01 java]# cat /etc/yum.repos.d/cloudera-manager.repo 
[cloudera-manager]
baseurl = http://192.168.60.71/cm/
gpgkey = http://192.168.60.71/cm/RPM-GPG-KEY-cloudera
gpgcheck = 1

[root@nn01 java]# cd /var/www/html/cm/
[root@nn01 cm]# ll
total 20
-rw-r--r-- 1 root root  488 May 14 21:24 cloudera-manager.repo
-rw-r--r-- 1 root root   57 May 14 21:14 mirrors
drwxr-xr-x 2 root root 4096 May 14 21:14 repodata
-rw-r--r-- 1 root root 1690 May 14 21:14 RPM-GPG-KEY-cloudera
drwxr-xr-x 3 root root 4096 May 14 21:14 RPMS
[root@nn01 cm]# 

[root@nn01 /]#yum install --assumeyes cloudera-manager-server-db-2
[root@nn01 /]#yum install --assumeyes cloudera-manager-daemons cloudera-manager-server

[root@nn01 cm]# service cloudera-scm-server-db status
pg_ctl: server is running (PID: 6941)
/usr/bin/postgres "-D" "/var/lib/cloudera-scm-server-db/data"
[root@nn01 cm]# service cloudera-scm-server status
cloudera-scm-server (pid  6979) is running...

On all nodes:
#yum install --assumeyes cloudera-manager-agent
