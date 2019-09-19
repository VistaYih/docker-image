FROM yishuida/galera

#COPY galera.repo /etc/yum.repos.d/

#RUN yum makecache && yum install -y galera-3 mysql-wsrep-5.7 rsync which

RUN rm -r /var/lib/mysql
COPY my.cnf /etc/mysql/my.cnf
COPY entrypoint.sh /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]