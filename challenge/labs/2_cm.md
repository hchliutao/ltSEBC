[root@node01 ~]# yum install -y cloudera-manager-server cloudera-manager-daemons cloudera-manager-agent<br>
Loaded plugins: fastestmirror, refresh-packagekit, security<br>
Loading mirror speeds from cached hostfile<br>
 * base: mirrors.aliyun.com<br>
 * extras: mirror.bit.edu.cn
 * updates: mirror.bit.edu.cn
cloudera-manager                                                                                               |  951 B     00:00 <br>    
cloudera-manager/primary                                                                                       | 4.1 kB     00:00  <br>   
cloudera-manager              <br>                                                                                                    7/7
Setting up Install Process<br>
Resolving Dependencies<br>
--> Running transaction check<br>
---> Package cloudera-manager-agent.x86_64 0:5.6.0-1.cm560.p0.54.el6 will be installed<br>
cloudera-manager/filelists                                                                                     |  96 kB     00:00     
--> Processing Dependency: mod_ssl for package: cloudera-manager-agent-5.6.0-1.cm560.p0.54.el6.x86_64<br>
--> Processing Dependency: MySQL-python for package: cloudera-manager-agent-5.6.0-1.cm560.p0.54.el6.x86_64<br>
--> Processing Dependency: python-psycopg2 for package: cloudera-manager-agent-5.6.0-1.cm560.p0.54.el6.x86_64<br>
--> Processing Dependency: openssl-devel for package: cloudera-manager-agent-5.6.0-1.cm560.p0.54.el6.x86_64<br>
---> Package cloudera-manager-daemons.x86_64 0:5.6.0-1.cm560.p0.54.el6 will be installed<br>
---> Package cloudera-manager-server.x86_64 0:5.6.0-1.cm560.p0.54.el6 will be installed<br>
--> Running transaction check<br>
---> Package MySQL-python.x86_64 0:1.2.3-0.3.c1.1.el6 will be installed<br>
---> Package mod_ssl.x86_64 1:2.2.15-47.el6.centos.4 will be installed<br>
--> Processing Dependency: httpd = 2.2.15-47.el6.centos.4 for package: 1:mod_ssl-2.2.15-47.el6.centos.4.x86_64<br>
---> Package openssl-devel.x86_64 0:1.0.1e-42.el6_7.4 will be installed<br>
--> Processing Dependency: openssl = 1.0.1e-42.el6_7.4 for package: openssl-devel-1.0.1e-42.el6_7.4.x86_64<br>
--> Processing Dependency: zlib-devel for package: openssl-devel-1.0.1e-42.el6_7.4.x86_64<br>
--> Processing Dependency: krb5-devel for package: openssl-devel-1.0.1e-42.el6_7.4.x86_64<br>
---> Package python-psycopg2.x86_64 0:2.0.14-2.el6 will be installed<br>
--> Running transaction check<br>
---> Package httpd.x86_64 0:2.2.15-29.el6.centos will be updated<br>
---> Package httpd.x86_64 0:2.2.15-47.el6.centos.4 will be an update<br>
--> Processing Dependency: httpd-tools = 2.2.15-47.el6.centos.4 for package: httpd-2.2.15-47.el6.centos.4.x86_64<br>
---> Package krb5-devel.x86_64 0:1.10.3-42z1.el6_7 will be installed<br>
--> Processing Dependency: krb5-libs = 1.10.3-42z1.el6_7 for package: krb5-devel-1.10.3-42z1.el6_7.x86_64<br>
--> Processing Dependency: libselinux-devel for package: krb5-devel-1.10.3-42z1.el6_7.x86_64<br>
--> Processing Dependency: libcom_err-devel for package: krb5-devel-1.10.3-42z1.el6_7.x86_64<br>
--> Processing Dependency: keyutils-libs-devel for package: krb5-devel-1.10.3-42z1.el6_7.x86_64<br>
---> Package openssl.x86_64 0:1.0.1e-15.el6 will be updated<br>
---> Package openssl.x86_64 0:1.0.1e-42.el6_7.4 will be an update<br>
---> Package zlib-devel.x86_64 0:1.2.3-29.el6 will be installed<br>
--> Running transaction check<br>
---> Package httpd-tools.x86_64 0:2.2.15-29.el6.centos will be updated<br>
---> Package httpd-tools.x86_64 0:2.2.15-47.el6.centos.4 will be an update<br>
---> Package keyutils-libs-devel.x86_64 0:1.4-5.el6 will be installed<br>
--> Processing Dependency: keyutils-libs = 1.4-5.el6 for package: keyutils-libs-devel-1.4-5.el6.x86_64<br>
---> Package krb5-libs.x86_64 0:1.10.3-10.el6_4.6 will be updated<br>
--> Processing Dependency: krb5-libs = 1.10.3-10.el6_4.6 for package: krb5-workstation-1.10.3-10.el6_4.6.x86_64<br>
---> Package krb5-libs.x86_64 0:1.10.3-42z1.el6_7 will be an update<br>
---> Package libcom_err-devel.x86_64 0:1.41.12-22.el6 will be installed<br>
--> Processing Dependency: libcom_err = 1.41.12-22.el6 for package: libcom_err-devel-1.41.12-22.el6.x86_64<br>
---> Package libselinux-devel.x86_64 0:2.0.94-5.8.el6 will be installed<br>
--> Processing Dependency: libselinux = 2.0.94-5.8.el6 for package: libselinux-devel-2.0.94-5.8.el6.x86_64<br>
--> Processing Dependency: libsepol-devel >= 2.0.32-1 for package: libselinux-devel-2.0.94-5.8.el6.x86_64<br>
--> Processing Dependency: pkgconfig(libsepol) for package: libselinux-devel-2.0.94-5.8.el6.x86_64<br>
--> Running transaction check<br>
---> Package keyutils-libs.x86_64 0:1.4-4.el6 will be updated<br>
--> Processing Dependency: keyutils-libs = 1.4-4.el6 for package: keyutils-1.4-4.el6.x86_64<br>
---> Package keyutils-libs.x86_64 0:1.4-5.el6 will be an update<br>
---> Package krb5-workstation.x86_64 0:1.10.3-10.el6_4.6 will be updated<br>
---> Package krb5-workstation.x86_64 0:1.10.3-42z1.el6_7 will be an update<br>
---> Package libcom_err.x86_64 0:1.41.12-18.el6 will be updated<br>
--> Processing Dependency: libcom_err = 1.41.12-18.el6 for package: e2fsprogs-libs-1.41.12-18.el6.x86_64<br>
--> Processing Dependency: libcom_err = 1.41.12-18.el6 for package: libss-1.41.12-18.el6.x86_64<br>
--> Processing Dependency: libcom_err = 1.41.12-18.el6 for package: e2fsprogs-1.41.12-18.el6.x86_64<br>
---> Package libcom_err.x86_64 0:1.41.12-22.el6 will be an update<br>
---> Package libselinux.x86_64 0:2.0.94-5.3.el6_4.1 will be updated<br>
--> Processing Dependency: libselinux = 2.0.94-5.3.el6_4.1 for package: libselinux-python-2.0.94-5.3.el6_4.1.x86_64<br>
--> Processing Dependency: libselinux = 2.0.94-5.3.el6_4.1 for package: libselinux-utils-2.0.94-5.3.el6_4.1.x86_64<br>
---> Package libselinux.x86_64 0:2.0.94-5.8.el6 will be an update<br>
---> Package libsepol-devel.x86_64 0:2.0.41-4.el6 will be installed<br>
--> Running transaction check<br>
---> Package e2fsprogs.x86_64 0:1.41.12-18.el6 will be updated<br>
---> Package e2fsprogs.x86_64 0:1.41.12-22.el6 will be an update<br>
---> Package e2fsprogs-libs.x86_64 0:1.41.12-18.el6 will be updated<br>
---> Package e2fsprogs-libs.x86_64 0:1.41.12-22.el6 will be an update<br>
---> Package keyutils.x86_64 0:1.4-4.el6 will be updated<br>
---> Package keyutils.x86_64 0:1.4-5.el6 will be an update<br>
---> Package libselinux-python.x86_64 0:2.0.94-5.3.el6_4.1 will be updated<br>
---> Package libselinux-python.x86_64 0:2.0.94-5.8.el6 will be an update<br>
---> Package libselinux-utils.x86_64 0:2.0.94-5.3.el6_4.1 will be updated<br>
---> Package libselinux-utils.x86_64 0:2.0.94-5.8.el6 will be an update<br>
---> Package libss.x86_64 0:1.41.12-18.el6 will be updated<br>
---> Package libss.x86_64 0:1.41.12-22.el6 will be an update<br>
--> Finished Dependency Resolution<br>

Dependencies Resolved

======================================================================================================================================
 Package                               Arch                Version                                Repository                     Size
======================================================================================================================================
Installing:
 cloudera-manager-agent                x86_64              5.6.0-1.cm560.p0.54.el6                cloudera-manager              4.7 M
 cloudera-manager-daemons              x86_64              5.6.0-1.cm560.p0.54.el6                cloudera-manager              474 M
 cloudera-manager-server               x86_64              5.6.0-1.cm560.p0.54.el6                cloudera-manager              8.2 k
Installing for dependencies:
 MySQL-python                          x86_64              1.2.3-0.3.c1.1.el6                     base                           86 k
 keyutils-libs-devel                   x86_64              1.4-5.el6                              base                           29 k
 krb5-devel                            x86_64              1.10.3-42z1.el6_7                      updates                       502 k
 libcom_err-devel                      x86_64              1.41.12-22.el6                         base                           33 k
 libselinux-devel                      x86_64              2.0.94-5.8.el6                         base                          137 k
 libsepol-devel                        x86_64              2.0.41-4.el6                           base                           64 k
 mod_ssl                               x86_64              1:2.2.15-47.el6.centos.4               updates                        95 k
 openssl-devel                         x86_64              1.0.1e-42.el6_7.4                      updates                       1.2 M
 python-psycopg2                       x86_64              2.0.14-2.el6                           base                          100 k
 zlib-devel                            x86_64              1.2.3-29.el6                           base                           44 k
Updating for dependencies:
 e2fsprogs                             x86_64              1.41.12-22.el6                         base                          554 k
 e2fsprogs-libs                        x86_64              1.41.12-22.el6                         base                          121 k
 httpd                                 x86_64              2.2.15-47.el6.centos.4                 updates                       831 k
 httpd-tools                           x86_64              2.2.15-47.el6.centos.4                 updates                        77 k
 keyutils                              x86_64              1.4-5.el6                              base                           39 k
 keyutils-libs                         x86_64              1.4-5.el6                              base                           20 k
 krb5-libs                             x86_64              1.10.3-42z1.el6_7                      updates                       769 k
 krb5-workstation                      x86_64              1.10.3-42z1.el6_7                      updates                       811 k
 libcom_err                            x86_64              1.41.12-22.el6                         base                           37 k
 libselinux                            x86_64              2.0.94-5.8.el6                         base                          108 k
 libselinux-python                     x86_64              2.0.94-5.8.el6                         base                          203 k
 libselinux-utils                      x86_64              2.0.94-5.8.el6                         base                           82 k
 libss                                 x86_64              1.41.12-22.el6                         base                           42 k
 openssl                               x86_64              1.0.1e-42.el6_7.4                      updates                       1.5 M

Transaction Summary
======================================================================================================================================
Install      13 Package(s)
Upgrade      14 Package(s)

Total download size: 486 M
Downloading Packages:
(1/27): MySQL-python-1.2.3-0.3.c1.1.el6.x86_64.rpm                                                             |  86 kB     00:00     
(2/27): cloudera-manager-agent-5.6.0-1.cm560.p0.54.el6.x86_64.rpm                                              | 4.7 MB     00:00     
(3/27): cloudera-manager-daemons-5.6.0-1.cm560.p0.54.el6.x86_64.rpm                                            | 474 MB     00:03     
(4/27): cloudera-manager-server-5.6.0-1.cm560.p0.54.el6.x86_64.rpm                                             | 8.2 kB     00:00     
(5/27): e2fsprogs-1.41.12-22.el6.x86_64.rpm                                                                    | 554 kB     00:00     
(6/27): e2fsprogs-libs-1.41.12-22.el6.x86_64.rpm                                                               | 121 kB     00:00     
(7/27): httpd-2.2.15-47.el6.centos.4.x86_64.rpm                                                                | 831 kB     00:01     
(8/27): httpd-tools-2.2.15-47.el6.centos.4.x86_64.rpm                                                          |  77 kB     00:00     
(9/27): keyutils-1.4-5.el6.x86_64.rpm                                                                          |  39 kB     00:00     
(10/27): keyutils-libs-1.4-5.el6.x86_64.rpm                                                                    |  20 kB     00:00     
(11/27): keyutils-libs-devel-1.4-5.el6.x86_64.rpm                                                              |  29 kB     00:00     
(12/27): krb5-devel-1.10.3-42z1.el6_7.x86_64.rpm                                                               | 502 kB     00:00     
(13/27): krb5-libs-1.10.3-42z1.el6_7.x86_64.rpm                                                                | 769 kB     00:01     
(14/27): krb5-workstation-1.10.3-42z1.el6_7.x86_64.rpm                                                         | 811 kB     00:00     
(15/27): libcom_err-1.41.12-22.el6.x86_64.rpm                                                                  |  37 kB     00:00     
(16/27): libcom_err-devel-1.41.12-22.el6.x86_64.rpm                                                            |  33 kB     00:00     
(17/27): libselinux-2.0.94-5.8.el6.x86_64.rpm                                                                  | 108 kB     00:00     
(18/27): libselinux-devel-2.0.94-5.8.el6.x86_64.rpm                                                            | 137 kB     00:00     
(19/27): libselinux-python-2.0.94-5.8.el6.x86_64.rpm                                                           | 203 kB     00:00     
(20/27): libselinux-utils-2.0.94-5.8.el6.x86_64.rpm                                                            |  82 kB     00:00     
(21/27): libsepol-devel-2.0.41-4.el6.x86_64.rpm                                                                |  64 kB     00:00     
(22/27): libss-1.41.12-22.el6.x86_64.rpm                                                                       |  42 kB     00:00     
(23/27): mod_ssl-2.2.15-47.el6.centos.4.x86_64.rpm                                                             |  95 kB     00:00     
(24/27): openssl-1.0.1e-42.el6_7.4.x86_64.rpm                                                                  | 1.5 MB     00:01     
(25/27): openssl-devel-1.0.1e-42.el6_7.4.x86_64.rpm                                                            | 1.2 MB     00:00     
(26/27): python-psycopg2-2.0.14-2.el6.x86_64.rpm                                                               | 100 kB     00:00     
(27/27): zlib-devel-1.2.3-29.el6.x86_64.rpm                                                                    |  44 kB     00:00     
--------------------------------------------------------------------------------------------------------------------------------------
Total                                                                                                  31 MB/s | 486 MB     00:15     
warning: rpmts_HdrFromFdno: Header V4 DSA/SHA1 Signature, key ID e8f86acd: NOKEY
Retrieving key from http://192.168.60.80/cm/RPM-GPG-KEY-cloudera
Importing GPG key 0xE8F86ACD:
 Userid: "Yum Maintainer <webmaster@cloudera.com>"
 From  : http://192.168.60.80/cm/RPM-GPG-KEY-cloudera
Running rpm_check_debug
Running Transaction Test
Transaction Test Succeeded
Running Transaction
Warning: RPMDB altered outside of yum.
** Found 3 pre-existing rpmdb problem(s), 'yum check' output follows:
1:libreoffice-core-4.0.4.2-9.el6.x86_64 has missing requires of libjawt.so()(64bit)
1:libreoffice-core-4.0.4.2-9.el6.x86_64 has missing requires of libjawt.so(SUNWprivate_1.1)(64bit)
1:libreoffice-ure-4.0.4.2-9.el6.x86_64 has missing requires of jre >= ('0', '1.5.0', None)
  Updating   : libcom_err-1.41.12-22.el6.x86_64                                                                                  1/41 
  Updating   : libselinux-2.0.94-5.8.el6.x86_64                                                                                  2/41 
  Updating   : keyutils-libs-1.4-5.el6.x86_64                                                                                    3/41 
  Updating   : krb5-libs-1.10.3-42z1.el6_7.x86_64                                                                                4/41 
  Updating   : openssl-1.0.1e-42.el6_7.4.x86_64                                                                                  5/41 
  Updating   : libss-1.41.12-22.el6.x86_64                                                                                       6/41 
  Installing : cloudera-manager-daemons-5.6.0-1.cm560.p0.54.el6.x86_64                                                           7/41 
  Installing : MySQL-python-1.2.3-0.3.c1.1.el6.x86_64                                                                            8/41 
  Updating   : httpd-tools-2.2.15-47.el6.centos.4.x86_64                                                                         9/41 
  Updating   : httpd-2.2.15-47.el6.centos.4.x86_64                                                                              10/41 
  Installing : 1:mod_ssl-2.2.15-47.el6.centos.4.x86_64                                                                          11/41 
  Installing : keyutils-libs-devel-1.4-5.el6.x86_64                                                                             12/41 
  Installing : libcom_err-devel-1.41.12-22.el6.x86_64                                                                           13/41 
  Updating   : e2fsprogs-libs-1.41.12-22.el6.x86_64                                                                             14/41 
  Installing : libsepol-devel-2.0.41-4.el6.x86_64                                                                               15/41 
  Installing : libselinux-devel-2.0.94-5.8.el6.x86_64                                                                           16/41 
  Installing : krb5-devel-1.10.3-42z1.el6_7.x86_64                                                                              17/41 
  Installing : zlib-devel-1.2.3-29.el6.x86_64                                                                                   18/41 
  Installing : openssl-devel-1.0.1e-42.el6_7.4.x86_64                                                                           19/41 
  Installing : python-psycopg2-2.0.14-2.el6.x86_64                                                                              20/41 
  Installing : cloudera-manager-agent-5.6.0-1.cm560.p0.54.el6.x86_64                                                            21/41 
  Updating   : e2fsprogs-1.41.12-22.el6.x86_64                                                                                  22/41 
  Installing : cloudera-manager-server-5.6.0-1.cm560.p0.54.el6.x86_64                                                           23/41 
  Updating   : krb5-workstation-1.10.3-42z1.el6_7.x86_64                                                                        24/41 
  Updating   : keyutils-1.4-5.el6.x86_64                                                                                        25/41 
  Updating   : libselinux-utils-2.0.94-5.8.el6.x86_64                                                                           26/41 
  Updating   : libselinux-python-2.0.94-5.8.el6.x86_64                                                                          27/41 
  Cleanup    : krb5-workstation-1.10.3-10.el6_4.6.x86_64                                                                        28/41 
  Cleanup    : e2fsprogs-1.41.12-18.el6.x86_64                                                                                  29/41 
  Cleanup    : httpd-2.2.15-29.el6.centos.x86_64                                                                                30/41 
  Cleanup    : httpd-tools-2.2.15-29.el6.centos.x86_64                                                                          31/41 
  Cleanup    : openssl-1.0.1e-15.el6.x86_64                                                                                     32/41 
  Cleanup    : krb5-libs-1.10.3-10.el6_4.6.x86_64                                                                               33/41 
  Cleanup    : e2fsprogs-libs-1.41.12-18.el6.x86_64                                                                             34/41 
  Cleanup    : libss-1.41.12-18.el6.x86_64                                                                                      35/41 
  Cleanup    : libselinux-python-2.0.94-5.3.el6_4.1.x86_64                                                                      36/41 
  Cleanup    : keyutils-1.4-4.el6.x86_64                                                                                        37/41 
  Cleanup    : libselinux-utils-2.0.94-5.3.el6_4.1.x86_64                                                                       38/41 
  Cleanup    : libselinux-2.0.94-5.3.el6_4.1.x86_64                                                                             39/41 
  Cleanup    : keyutils-libs-1.4-4.el6.x86_64                                                                                   40/41 
  Cleanup    : libcom_err-1.41.12-18.el6.x86_64                                                                                 41/41 
  Verifying  : krb5-devel-1.10.3-42z1.el6_7.x86_64                                                                               1/41 
  Verifying  : krb5-libs-1.10.3-42z1.el6_7.x86_64                                                                                2/41 
  Verifying  : libselinux-utils-2.0.94-5.8.el6.x86_64                                                                            3/41 
  Verifying  : httpd-2.2.15-47.el6.centos.4.x86_64                                                                               4/41 
  Verifying  : python-psycopg2-2.0.14-2.el6.x86_64                                                                               5/41 
  Verifying  : keyutils-libs-devel-1.4-5.el6.x86_64                                                                              6/41 
  Verifying  : libss-1.41.12-22.el6.x86_64                                                                                       7/41 
  Verifying  : MySQL-python-1.2.3-0.3.c1.1.el6.x86_64                                                                            8/41 
  Verifying  : krb5-workstation-1.10.3-42z1.el6_7.x86_64                                                                         9/41 
  Verifying  : zlib-devel-1.2.3-29.el6.x86_64                                                                                   10/41 
  Verifying  : openssl-devel-1.0.1e-42.el6_7.4.x86_64                                                                           11/41 
  Verifying  : cloudera-manager-server-5.6.0-1.cm560.p0.54.el6.x86_64                                                           12/41 
  Verifying  : keyutils-libs-1.4-5.el6.x86_64                                                                                   13/41 
  Verifying  : cloudera-manager-agent-5.6.0-1.cm560.p0.54.el6.x86_64                                                            14/41 
  Verifying  : libcom_err-devel-1.41.12-22.el6.x86_64                                                                           15/41 
  Verifying  : keyutils-1.4-5.el6.x86_64                                                                                        16/41 
  Verifying  : cloudera-manager-daemons-5.6.0-1.cm560.p0.54.el6.x86_64                                                          17/41 
  Verifying  : e2fsprogs-1.41.12-22.el6.x86_64                                                                                  18/41 
  Verifying  : 1:mod_ssl-2.2.15-47.el6.centos.4.x86_64                                                                          19/41 
  Verifying  : libsepol-devel-2.0.41-4.el6.x86_64                                                                               20/41 
  Verifying  : libselinux-2.0.94-5.8.el6.x86_64                                                                                 21/41 
  Verifying  : httpd-tools-2.2.15-47.el6.centos.4.x86_64                                                                        22/41 
  Verifying  : libselinux-devel-2.0.94-5.8.el6.x86_64                                                                           23/41 
  Verifying  : libcom_err-1.41.12-22.el6.x86_64                                                                                 24/41 
  Verifying  : libselinux-python-2.0.94-5.8.el6.x86_64                                                                          25/41 
  Verifying  : e2fsprogs-libs-1.41.12-22.el6.x86_64                                                                             26/41 
  Verifying  : openssl-1.0.1e-42.el6_7.4.x86_64                                                                                 27/41 
  Verifying  : httpd-2.2.15-29.el6.centos.x86_64                                                                                28/41 
  Verifying  : e2fsprogs-1.41.12-18.el6.x86_64                                                                                  29/41 
  Verifying  : libselinux-2.0.94-5.3.el6_4.1.x86_64                                                                             30/41 
  Verifying  : openssl-1.0.1e-15.el6.x86_64                                                                                     31/41 
  Verifying  : libselinux-utils-2.0.94-5.3.el6_4.1.x86_64                                                                       32/41 
  Verifying  : libss-1.41.12-18.el6.x86_64                                                                                      33/41 
  Verifying  : libcom_err-1.41.12-18.el6.x86_64                                                                                 34/41 
  Verifying  : e2fsprogs-libs-1.41.12-18.el6.x86_64                                                                             35/41 
  Verifying  : libselinux-python-2.0.94-5.3.el6_4.1.x86_64                                                                      36/41 
  Verifying  : krb5-libs-1.10.3-10.el6_4.6.x86_64                                                                               37/41 
  Verifying  : keyutils-1.4-4.el6.x86_64                                                                                        38/41 
  Verifying  : httpd-tools-2.2.15-29.el6.centos.x86_64                                                                          39/41 
  Verifying  : krb5-workstation-1.10.3-10.el6_4.6.x86_64                                                                        40/41 
  Verifying  : keyutils-libs-1.4-4.el6.x86_64                                                                                   41/41 

Installed:
  cloudera-manager-agent.x86_64 0:5.6.0-1.cm560.p0.54.el6           cloudera-manager-daemons.x86_64 0:5.6.0-1.cm560.p0.54.el6         
  cloudera-manager-server.x86_64 0:5.6.0-1.cm560.p0.54.el6         

Dependency Installed:
  MySQL-python.x86_64 0:1.2.3-0.3.c1.1.el6     keyutils-libs-devel.x86_64 0:1.4-5.el6       krb5-devel.x86_64 0:1.10.3-42z1.el6_7    
  libcom_err-devel.x86_64 0:1.41.12-22.el6     libselinux-devel.x86_64 0:2.0.94-5.8.el6     libsepol-devel.x86_64 0:2.0.41-4.el6     
  mod_ssl.x86_64 1:2.2.15-47.el6.centos.4      openssl-devel.x86_64 0:1.0.1e-42.el6_7.4     python-psycopg2.x86_64 0:2.0.14-2.el6    
  zlib-devel.x86_64 0:1.2.3-29.el6            

Dependency Updated:
  e2fsprogs.x86_64 0:1.41.12-22.el6            e2fsprogs-libs.x86_64 0:1.41.12-22.el6       httpd.x86_64 0:2.2.15-47.el6.centos.4    
  httpd-tools.x86_64 0:2.2.15-47.el6.centos.4  keyutils.x86_64 0:1.4-5.el6                  keyutils-libs.x86_64 0:1.4-5.el6         
  krb5-libs.x86_64 0:1.10.3-42z1.el6_7         krb5-workstation.x86_64 0:1.10.3-42z1.el6_7  libcom_err.x86_64 0:1.41.12-22.el6       
  libselinux.x86_64 0:2.0.94-5.8.el6           libselinux-python.x86_64 0:2.0.94-5.8.el6    libselinux-utils.x86_64 0:2.0.94-5.8.el6 
  libss.x86_64 0:1.41.12-22.el6                openssl.x86_64 0:1.0.1e-42.el6_7.4          

Complete!

----------------------------------------
[root@node01 ~]# /usr/share/cmf/schema/scm_prepare_database.sh mysql -h 192.168.60.70 --scm-host localhost scm scm 123456<br>
JAVA_HOME=/usr/java/latest/<br>
Verifying that we can write to /etc/cloudera-scm-server<br>
Creating SCM configuration file in /etc/cloudera-scm-server<br>
Executing:  /usr/java/latest//bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
[                          main] DbCommandExecutor              INFO  Successfully connected to database.
All done, your SCM database is configured correctly!
[root@node01 ~]# 
