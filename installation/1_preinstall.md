
vi /etc/sysconfig/network
HOSTNAME=xxxxx<br>
#hostname xxxx<br>

# vi /etc/hosts
192.168.60.71 nn01
192.168.60.72 nn02
192.168.60.73 dn01
192.168.60.74 dn02
192.168.60.75 dn03


# service iptables stop
# chkconfig iptables off 
# vi /etc/selinux/config 
   SELINUX=disabled
# service network restart
# /etc/init.d/network restart


# yum install ntp
# service ntpd start
# chkconfig ntpd on

# ntpdate -u 202.108.6.95
# vi /etc/ntp.conf
  server 202.108.6.95 prefer
# service ntpd start
# chkconfig ntpd on

install JDK:
#rpm -ivh jdk-7u55-linux-x64.rpm
#rpm -ivh oracle-j2sdk1.7-1.7.0 update67-1.x86_64.rpm
#yum install --assumeyes cloudera-manager-server-db-2
#yum install --assumeyes cloudera-manager-daemons cloudera-manager-server

[root@nn01 ~]# yum install --assumeyes cloudera-manager-daemons cloudera-manager-server
Loaded plugins: fastestmirror, refresh-packagekit, security
Loading mirror speeds from cached hostfile
* base: mirrors.aliyun.com
* extras: mirrors.aliyun.com
* updates: mirrors.pubyun.com
Setting up Install Process
Resolving Dependencies
--> Running transaction check
---> Package cloudera-manager-daemons.x86_64 0:5.7.0-1.cm570.p0.76.el6 will be installed
---> Package cloudera-manager-server.x86_64 0:5.7.0-1.cm570.p0.76.el6 will be installed
--> Finished Dependency Resolution

Dependencies Resolved

============================================================================================
Package                     Arch      Version                    Repository           Size
============================================================================================
Installing:
cloudera-manager-daemons    x86_64    5.7.0-1.cm570.p0.76.el6    cloudera-manager    539 M
cloudera-manager-server     x86_64    5.7.0-1.cm570.p0.76.el6    cloudera-manager    8.2 k

Transaction Summary
============================================================================================
Install       2 Package(s)

Total size: 539 M
Total download size: 539 M
Installed size: 861 M
Downloading Packages:
cloudera-manager-daemons-5.7.0-1.cm570.p0.76.el6.x86_64.rpm          | 539 MB     05:48    
Running rpm_check_debug
Running Transaction Test
Transaction Test Succeeded
Running Transaction
  Installing : cloudera-manager-daemons-5.7.0-1.cm570.p0.76.el6.x86_64                  1/2
  Installing : cloudera-manager-server-5.7.0-1.cm570.p0.76.el6.x86_64                   2/2
  Verifying  : cloudera-manager-server-5.7.0-1.cm570.p0.76.el6.x86_64                   1/2
  Verifying  : cloudera-manager-daemons-5.7.0-1.cm570.p0.76.el6.x86_64                  2/2

Installed:
  cloudera-manager-daemons.x86_64 0:5.7.0-1.cm570.p0.76.el6                                
  cloudera-manager-server.x86_64 0:5.7.0-1.cm570.p0.76.el6                                 

Complete!
[root@myhost-1 ~]# 

install CM-agent:

#yum install --assumeyes cloudera-manager-agent
