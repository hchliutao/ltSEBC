[root@nn01 /]# cat /etc/sysctl.conf | grep vm.swappiness<br>
vm.swappiness = 1<br>
[root@nn01 /]# <br>
<br>
[root@nn01 /]# service ntpd status<br>
ntpd (pid  1909) is running...<br>
[root@nn01 /]# <br>
<br>
[root@nn01 /]# cat /etc/sysconfig/network<br>
NETWORKING=yes<br>
HOSTNAME=nn01<br>
NETWORKING_IPV6=no<br>
NETMASK=255.255.255.0<br>
GATEWAY=192.168.60.254<br>
DNS1=202.102.152.3<br>
<br>
[root@nn01 /]# cat /etc/hosts<br>
192.168.60.71 nn01<br>
192.168.60.72 nn02<br>
192.168.60.73 dn01<br>
192.168.60.74 dn02<br>
192.168.60.75 dn03<br>

[root@nn01 /]# service iptables status<br>
iptables: Firewall is not running.<br>
[root@nn01 /]# <br>

[root@nn01 /]# cat /etc/selinux/config  | grep SELINUX<br>
SELINUX=disabled<br>

[root@nn01 /]# cd /var/www/html/java/<br>
[root@nn01 java]# pwd<br>
/var/www/html/java<br>

[root@nn01 java]# ll<br>
total 258496<br>
-rw-r--r-- 1 root root 122656363 May 14 21:14 jdk-7u55-linux-x64.rpm<br>
-rw-r--r-- 1 root root 142039186 May 14 21:14 oracle-j2sdk1.7-1.7.0 update67-1.x86_64.rpm<br>
[root@nn01 java]# rpm -ivh jdk-7u55-linux-x64.rpm<br>
[root@nn01 java]#rpm -ivh oracle-j2sdk1.7-1.7.0 update67-1.x86_64.rpm<br>

[root@nn01 /]# java -version<br>
java version "1.7.0_55"<br>
Java(TM) SE Runtime Environment (build 1.7.0_55-b13)<br>
Java HotSpot(TM) 64-Bit Server VM (build 24.55-b03, mixed mode)<br>
[root@nn01 /]# <br>

[root@nn01 java]# cat /etc/yum.repos.d/cloudera-manager.repo <br>
[cloudera-manager]<br>
baseurl = http://192.168.60.71/cm/<br>
gpgkey = http://192.168.60.71/cm/RPM-GPG-KEY-cloudera<br>
gpgcheck = 1<br>

[root@nn01 java]# cd /var/www/html/cm/<br>
[root@nn01 cm]# ll<br>
total 20<br>
-rw-r--r-- 1 root root  488 May 14 21:24 cloudera-manager.repo<br>
-rw-r--r-- 1 root root   57 May 14 21:14 mirrors<br>
drwxr-xr-x 2 root root 4096 May 14 21:14 repodata<br>
-rw-r--r-- 1 root root 1690 May 14 21:14 RPM-GPG-KEY-cloudera<br>
drwxr-xr-x 3 root root 4096 May 14 21:14 RPMS<br>
[root@nn01 cm]# <br>

[root@nn01 /]#yum install --assumeyes cloudera-manager-server-db-2<br>
[root@nn01 /]#yum install --assumeyes cloudera-manager-daemons cloudera-manager-server<br>

[root@nn01 cm]# service cloudera-scm-server-db status<br>
pg_ctl: server is running (PID: 6941)<br>
/usr/bin/postgres "-D" "/var/lib/cloudera-scm-server-db/data"<br>
[root@nn01 cm]# service cloudera-scm-server status<br>
cloudera-scm-server (pid  6979) is running...<br>

On all nodes:<br>
#yum install --assumeyes cloudera-manager-agent<br>
