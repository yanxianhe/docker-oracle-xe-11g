docker-oracle-xe-11g
============================
[![](https://badge.imagelayers.io/sath89/oracle-xe-11g:latest.svg)](https://imagelayers.io/?images=sath89/oracle-xe-11g:latest 'Get your own badge on imagelayers.io')

Oracle Express Edition 11g Release 2 on Ubuntu 14.04.1 LTS

This **Dockerfile** is a [trusted build](https://registry.hub.docker.com/u/sath89/oracle-xe-11g/) of [Docker Registry](https://registry.hub.docker.com/).


##### win10 docker 运行

~~~~~~
docker run --name oracle -p 8080:8080 -p 1521:1521 -v D:\opt\docker\oracle:/u01/app/oracle  -d registry.cn-beijing.aliyuncs.com/dockermg/oracle-xe:0.2.0
~~~~~~

##### 登录

~~~~~~
http://127.0.0.1:8080/apex
workspace: INTERNAL
user: ADMIN
password: oracle

hostname: 127.0.0.1
port: 1521
sid: xe
username: system
password: oracle

pl/sql 127.0.0.1:1521/XE

~~~~~~


##### 使用管理员直接进入


~~~~~~
su oracle -c "NLS_LANG=.$CHARACTER_SET $ORACLE_HOME/bin/sqlplus / as sysdba"
~~~~~~



