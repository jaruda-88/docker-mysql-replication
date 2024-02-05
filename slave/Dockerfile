FROM mysql_image:slave
MAINTAINER ljm

USER root
RUN echo "slave" > slave.txt

ADD my.cnf /engn001/mysql/
ADD docker_entrypoint.sh /usr/local/bin
ADD chmod 640 /engn001/mysql/my.cnf
ADD chmod 755 /urs/local/bin/docker-entrypoint.sh

ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]