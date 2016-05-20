 -----------------------<br>
 [root@mysql ~]# yum repolist enabled<br>
Loaded plugins: fastestmirror, refresh-packagekit, security<br>
Loading mirror speeds from cached hostfile<br>
 * base: mirror.bit.edu.cn<br>
 * extras: mirror.bit.edu.cn<br>
 * updates: mirror.bit.edu.cn<br>
repo id                                              repo name                                                     status<br>
base                                                 CentOS-6 - Base                                               6,575<br>
extras                                               CentOS-6 - Extras                                                62<br>
mysql56-community                                    MySQL 5.6 Community Server                                      248<br>
updates                                              CentOS-6 - Updates                                            1,622<br>
repolist: 8,507
[root@mysql ~]# <br>

-----------------------------------<br>
[root@mysql ~]# yum install -y mysql-community-devel mysql-community-server mysql-community-client mysql-community-common<br> mysql-community-libs<br>
Loaded plugins: fastestmirror, refresh-packagekit, security<br>
Loading mirror speeds from cached hostfile<br>
 * base: mirror.bit.edu.cn<br>
 * extras: mirror.bit.edu.cn<br>
 * updates: mirror.bit.edu.cn<br>
Setting up Install Process<br>
Resolving Dependencies<br>
--> Running transaction check<br>
---> Package mysql.x86_64 0:5.1.71-1.el6 will be obsoleted<br>
---> Package mysql-community-client.x86_64 0:5.6.30-2.el6 will be obsoleting<br>
---> Package mysql-community-common.x86_64 0:5.6.30-2.el6 will be installed<br>
---> Package mysql-community-devel.x86_64 0:5.6.30-2.el6 will be installed<br>
---> Package mysql-community-libs.x86_64 0:5.6.30-2.el6 will be obsoleting<br>
---> Package mysql-community-server.x86_64 0:5.6.30-2.el6 will be obsoleting<br>
---> Package mysql-libs.x86_64 0:5.1.71-1.el6 will be obsoleted<br>
--> Processing Dependency: libmysqlclient.so.16()(64bit) for package: 2:postfix-2.6.6-2.2.el6_1.x86_64<br>
--> Processing Dependency: libmysqlclient.so.16()(64bit) for package: redland-1.0.7-11.el6.x86_64<br>
--> Processing Dependency: libmysqlclient.so.16()(64bit) for package: perl-DBD-MySQL-4.013-3.el6.x86_64<br>
--> Processing Dependency: libmysqlclient.so.16(libmysqlclient_16)(64bit) for package: 2:postfix-2.6.6-2.2.el6_1.x86_64<br>
--> Processing Dependency: libmysqlclient.so.16(libmysqlclient_16)(64bit) for package: redland-1.0.7-11.el6.x86_64<br>
--> Processing Dependency: libmysqlclient.so.16(libmysqlclient_16)(64bit) for package: perl-DBD-MySQL-4.013-3.el6.x86_64<br>
--> Processing Dependency: libmysqlclient_r.so.16()(64bit) for package: 1:qt-mysql-4.6.2-26.el6_4.x86_64<br>
--> Processing Dependency: libmysqlclient_r.so.16(libmysqlclient_16)(64bit) for package: 1:qt-mysql-4.6.2-26.el6_4.x86_64<br>
---> Package mysql-server.x86_64 0:5.1.71-1.el6 will be obsoleted<br>
--> Running transaction check<br>
---> Package mysql-community-libs-compat.x86_64 0:5.6.30-2.el6 will be obsoleting<br>
---> Package postfix.x86_64 2:2.6.6-2.2.el6_1 will be updated<br>
---> Package postfix.x86_64 2:2.6.6-6.el6_7.1 will be an update<br>
---> Package qt-mysql.x86_64 1:4.6.2-26.el6_4 will be updated<br>
---> Package qt-mysql.x86_64 1:4.6.2-28.el6_5 will be an update<br>
--> Processing Dependency: qt(x86-64) = 1:4.6.2-28.el6_5 for package: 1:qt-mysql-4.6.2-28.el6_5.x86_64<br>
--> Running transaction check<br>
---> Package qt.x86_64 1:4.6.2-26.el6_4 will be updated<br>
--> Processing Dependency: qt(x86-64) = 1:4.6.2-26.el6_4 for package: 1:qt-sqlite-4.6.2-26.el6_4.x86_64<br>
--> Processing Dependency: qt(x86-64) = 1:4.6.2-26.el6_4 for package: 1:qt-x11-4.6.2-26.el6_4.x86_64<br>
---> Package qt.x86_64 1:4.6.2-28.el6_5 will be an update<br>
--> Running transaction check<br>
---> Package qt-sqlite.x86_64 1:4.6.2-26.el6_4 will be updated<br>
---> Package qt-sqlite.x86_64 1:4.6.2-28.el6_5 will be an update<br>
---> Package qt-x11.x86_64 1:4.6.2-26.el6_4 will be updated<br>
---> Package qt-x11.x86_64 1:4.6.2-28.el6_5 will be an update<br>
--> Finished Dependency Resolution<br>

Dependencies Resolved<br>

=========================================================================================================================
 Package                               Arch             Version                        Repository                   Size
=========================================================================================================================
Installing:
 mysql-community-client                x86_64           5.6.30-2.el6                   mysql56-community            18 M
     replacing  mysql.x86_64 5.1.71-1.el6
 mysql-community-common                x86_64           5.6.30-2.el6                   mysql56-community           308 k
 mysql-community-devel                 x86_64           5.6.30-2.el6                   mysql56-community           3.3 M
 mysql-community-libs                  x86_64           5.6.30-2.el6                   mysql56-community           1.9 M
     replacing  mysql-libs.x86_64 5.1.71-1.el6
 mysql-community-libs-compat           x86_64           5.6.30-2.el6                   mysql56-community           1.6 M
     replacing  mysql-libs.x86_64 5.1.71-1.el6
 mysql-community-server                x86_64           5.6.30-2.el6                   mysql56-community            54 M
     replacing  mysql-server.x86_64 5.1.71-1.el6
Updating for dependencies:
 postfix                               x86_64           2:2.6.6-6.el6_7.1              updates                     2.0 M
 qt                                    x86_64           1:4.6.2-28.el6_5               base                        3.9 M
 qt-mysql                              x86_64           1:4.6.2-28.el6_5               base                         59 k
 qt-sqlite                             x86_64           1:4.6.2-28.el6_5               base                         51 k
 qt-x11                                x86_64           1:4.6.2-28.el6_5               base                         12 M

Transaction Summary
=========================================================================================================================
Install       6 Package(s)<br>
Upgrade       5 Package(s)<br>

Total size: 97 M<br>
Downloading Packages:<br>
warning: rpmts_HdrFromFdno: Header V3 DSA/SHA1 Signature, key ID 5072e1f5: NOKEY<br>
Retrieving key from file:/etc/pki/rpm-gpg/RPM-GPG-KEY-mysql<br>
Importing GPG key 0x5072E1F5:<br>
 Userid : MySQL Release Engineering <mysql-build@oss.oracle.com><br>
 Package: mysql-community-release-el6-5.noarch (installed)<br>
 From   : file:/etc/pki/rpm-gpg/RPM-GPG-KEY-mysql<br>
Running rpm_check_debug<br>
Running Transaction Test<br>
Transaction Test Succeeded<br>
Running Transaction<br>
Warning: RPMDB altered outside of yum.<br>
** Found 3 pre-existing rpmdb problem(s), 'yum check' output follows:<br>
1:libreoffice-core-4.0.4.2-9.el6.x86_64 has missing requires of libjawt.so()(64bit)<br>
1:libreoffice-core-4.0.4.2-9.el6.x86_64 has missing requires of libjawt.so(SUNWprivate_1.1)(64bit)<br>
1:libreoffice-ure-4.0.4.2-9.el6.x86_64 has missing requires of jre >= ('0', '1.5.0', None)<br>
  Updating   : 1:qt-4.6.2-28.el6_5.x86_64                                                                           1/19 <br>
  Installing : mysql-community-common-5.6.30-2.el6.x86_64                                                           2/19 <br>
  Installing : mysql-community-libs-5.6.30-2.el6.x86_64                                                             3/19 <br>
  Installing : mysql-community-libs-compat-5.6.30-2.el6.x86_64                                                      4/19 <br>
  Installing : mysql-community-client-5.6.30-2.el6.x86_64                                                           5/19 <br>
  Updating   : 1:qt-sqlite-4.6.2-28.el6_5.x86_64                                                                    6/19 <br>
  Updating   : 1:qt-x11-4.6.2-28.el6_5.x86_64                                                                       7/19 <br>
  Installing : mysql-community-server-5.6.30-2.el6.x86_64                                                           8/19 <br>
  Updating   : 2:postfix-2.6.6-6.el6_7.1.x86_64                                                                     9/19 <br>
  Updating   : 1:qt-mysql-4.6.2-28.el6_5.x86_64                                                                    10/19 <br>
  Installing : mysql-community-devel-5.6.30-2.el6.x86_64                                                           11/19 <br>
  Cleanup    : 1:qt-mysql-4.6.2-26.el6_4.x86_64                                                                    12/19 <br>
  Cleanup    : 1:qt-x11-4.6.2-26.el6_4.x86_64                                                                      13/19 <br>
  Erasing    : mysql-server-5.1.71-1.el6.x86_64                                                                    14/19 <br>
  Erasing    : mysql-5.1.71-1.el6.x86_64                                                                           15/19 <br>
  Cleanup    : 1:qt-sqlite-4.6.2-26.el6_4.x86_64                                                                   16/19 <br><br>
  Cleanup    : 2:postfix-2.6.6-2.2.el6_1.x86_64                                                                    17/19 <br>
  Erasing    : mysql-libs-5.1.71-1.el6.x86_64                                                                      18/19 <br>
  Cleanup    : 1:qt-4.6.2-26.el6_4.x86_64                                                                          19/19 <br>
  Verifying  : mysql-community-libs-compat-5.6.30-2.el6.x86_64                                                      1/19 <br>
  Verifying  : mysql-community-devel-5.6.30-2.el6.x86_64                                                            2/19 <br>
  Verifying  : mysql-community-server-5.6.30-2.el6.x86_64                                                           3/19 <br>
  Verifying  : 2:postfix-2.6.6-6.el6_7.1.x86_64                                                                     4/19 <br>
  Verifying  : 1:qt-4.6.2-28.el6_5.x86_64                                                                           5/19 <br>
  Verifying  : mysql-community-client-5.6.30-2.el6.x86_64                                                           6/19 <br>
  Verifying  : 1:qt-mysql-4.6.2-28.el6_5.x86_64                                                                     7/19 <br>
  Verifying  : 1:qt-x11-4.6.2-28.el6_5.x86_64                                                                       8/19 <br>
  Verifying  : mysql-community-libs-5.6.30-2.el6.x86_64                                                             9/19 <br>
  Verifying  : mysql-community-common-5.6.30-2.el6.x86_64                                                          10/19 <br>
  Verifying  : 1:qt-sqlite-4.6.2-28.el6_5.x86_64                                                                   11/19 <br>
  Verifying  : 1:qt-x11-4.6.2-26.el6_4.x86_64                                                                      12/19 <br>
  Verifying  : 1:qt-sqlite-4.6.2-26.el6_4.x86_64                                                                   13/19 <br>
  Verifying  : 2:postfix-2.6.6-2.2.el6_1.x86_64                                                                    14/19 <br>
  Verifying  : mysql-libs-5.1.71-1.el6.x86_64                                                                      15/19 <br>
  Verifying  : 1:qt-4.6.2-26.el6_4.x86_64                                                                          16/19 <br>
  Verifying  : mysql-server-5.1.71-1.el6.x86_64                                                                    17/19 <br>
  Verifying  : mysql-5.1.71-1.el6.x86_64                                                                           18/19 <br>
  Verifying  : 1:qt-mysql-4.6.2-26.el6_4.x86_64                                                                    19/19 <br>

Installed:
  mysql-community-client.x86_64 0:5.6.30-2.el6                  mysql-community-common.x86_64 0:5.6.30-2.el6       <br>     
  mysql-community-devel.x86_64 0:5.6.30-2.el6                   mysql-community-libs.x86_64 0:5.6.30-2.el6             <br> 
  mysql-community-libs-compat.x86_64 0:5.6.30-2.el6             mysql-community-server.x86_64 0:5.6.30-2.el6            <br>

Dependency Updated:<br>
  postfix.x86_64 2:2.6.6-6.el6_7.1         qt.x86_64 1:4.6.2-28.el6_5            qt-mysql.x86_64 1:4.6.2-28.el6_5   <br>    
  qt-sqlite.x86_64 1:4.6.2-28.el6_5        qt-x11.x86_64 1:4.6.2-28.el6_5       <br>

Replaced:
  mysql.x86_64 0:5.1.71-1.el6         mysql-libs.x86_64 0:5.1.71-1.el6         mysql-server.x86_64 0:5.1.71-1.el6     <br>   

Complete!<br>

-------------------------<br>
#Create database
# mysql -u root --password='123456' -e "create user 'scm'@'%' identified by '123456'" <br>
# mysql -u root --password='123456' -e 'create database scm default character set utf8' <br>
# mysql -u root --password='123456' -e "grant all privileges on scm.* to 'scm'@'%'"<br>

# mysql -u root --password='123456' -e "create user 'rman'@'%' identified by '123456'" <br>
# mysql -u root --password='123456' -e 'create database rman default character set utf8' <br>
# mysql -u root --password='123456' -e "grant all privileges on rman.* to 'rman'@'%'" <br>

# mysql -u root --password='123456' -e "create user 'hivey'@'%' identified by '123456'"<br>
# mysql -u root --password='123456' -e 'create database hivey default character set utf8'<br>
# mysql -u root --password='123456' -e "grant all privileges on hivey.* to 'hivey'@'%'"<br>

# mysql -u root --password='123456' -e "create user 'oozie'@'%' identified by '123456'" <br>
# mysql -u root --password='123456' -e 'create database oozie default character set utf8' <br>
# mysql -u root --password='123456' -e "grant all privileges on oozie.* to 'oozie'@'%'"<br> 

# mysql -u root --password='123456' -e "create user 'huey'@'%' identified by '123456'" <br>
# mysql -u root --password='123456' -e 'create database huey default character set utf8'<br>
# mysql -u root --password='123456' -e "grant all privileges on huey.* to 'huey'@'%'"<br>


[root@mysql ~]# mysql --version<br>
mysql  Ver 14.14 Distrib 5.6.30, for Linux (x86_64) using  EditLine wrapper<br>
[root@mysql ~]# <br>


mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hivey              |
| huey               |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
+--------------------+
8 rows in set (0.00 sec)

mysql> 
