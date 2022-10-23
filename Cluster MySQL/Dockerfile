# Galera Cluster Dockerfile
FROM debian

RUN apt update && apt -y upgrade && apt -y dist-upgrade && apt -y autoremove

RUN apt install -y build-essential systemctl mariadb-server mariadb-client rsync 

COPY 60-galera.cnf /etc/mysql/mariadb.conf.d/
COPY 50-server.cnf /etc/mysql/mariadb.conf.d/

RUN chmod 777 -R /etc/mysql/mariadb.conf.d/

