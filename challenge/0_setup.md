[root@node01 .ssh]# cat /etc/hosts<br>
127.0.0.1   localhost localhost.localdomain localhost4 localhost4.localdomain4<br>
::1         localhost localhost.localdomain localhost6 localhost6.localdomain6<br>

192.168.60.70 mysql<br>
192.168.60.71 node01<br>
192.168.60.72 node02<br>
192.168.60.73 node03<br>
192.168.60.74 node04<br>
192.168.60.75 node05<br>
--------------------------------------------------------

[root@node01 ~]# lsb_release -a<br>
LSB Version:	:base-4.0-amd64:base-4.0-noarch:core-4.0-amd64:core-4.0-noarch:graphics-4.0-amd64:graphics-4.0-noarch:printing-4.0-amd64:printing-4.0-noarch<br>
Distributor ID:	CentOS<br>
Description:	CentOS release 6.5 (Final)<br>
Release:	6.5<br>
Codename:	Final<br>
[root@node01 ~]# <br>
----------------------------------------------------

[root@node01 ~]# uptime<br>
 07:46:08 up 4 min,  1 user,  load average: 0.01, 0.08, 0.04<br>
[root@node01 ~]# <br>

------------------------------------------------------

[root@node01 .ssh]# ll /etc/yum.repos.d/<br>
total 16<br>
-rw-r--r--. 1 root root 1926 Nov 27  2013 CentOS-Base.repo<br>
-rw-r--r--. 1 root root  638 Nov 27  2013 CentOS-Debuginfo.repo<br>
-rw-r--r--. 1 root root  630 Nov 27  2013 CentOS-Media.repo<br>
-rw-r--r--. 1 root root 3664 Nov 27  2013 CentOS-Vault.repo<br>
[root@node01 .ssh]# <br>

-------------------------------------------------

[root@node01 ~]# useradd -u 2200 yaoming <br>
[root@node01 ~]# useradd -u 2300 jetli <br>
[root@node01 ~]# groupadd shanghai <br>
[root@node01 ~]# groupadd beijing <br>
[root@node01 ~]# gpasswd -a yaoming shanghai <br>
Adding user yaoming to group shanghai <br>
[root@node01 ~]# gpasswd -a jetli beijing <br>
Adding user jetli to group beijing <br>
[root@node01 ~]#  <br>

[root@node01 ~]# cat /etc/passwd | grep yaoming <br>
yaoming:x:2200:2200::/home/yaoming:/bin/bash <br>
[root@node01 ~]# cat /etc/passwd | grep jetli <br>
jetli:x:2300:2300::/home/jetli:/bin/bash <br>
[root@node01 ~]# cat /etc/group | grep shanghai <br>
shanghai:x:2301:yaoming <br>
[root@node01 ~]# cat /etc/group | grep beijing <br>
beijing:x:2302:jetli <br>
[root@node01 ~]#  <br>




