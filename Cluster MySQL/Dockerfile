# Galera Cluster Dockerfile
FROM mariadb:10.6.8-focal

RUN apt update && apt -y upgrade && apt -y dist-upgrade && apt -y autoremove

RUN apt -y install build-essential tcl systemctl

COPY 60-galera.cnf /etc/mysql/mariadb.conf.d/

