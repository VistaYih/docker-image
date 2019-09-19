FROM centos:7

COPY galera.repo /etc/yum.repos.d/

RUN yum makecache && yum install -y galera-3 mysql-wsrep-5.7 rsync which