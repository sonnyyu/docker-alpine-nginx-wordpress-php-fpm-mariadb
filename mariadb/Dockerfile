FROM alpine:3.9

MAINTAINER Sonny Yu <sonnyyuirm@gmail.com>

RUN apk add --no-cache mariadb mariadb-client mariadb-server-utils pwgen tzdata && \
    rm -f /var/cache/apk/* /tmp/*
    
ENV  TZ=America/Los_Angeles

ADD install.sh /scripts/install.sh
ADD world.sql  /scripts/world.sql
RUN mkdir /docker-entrypoint-initdb.d && \
    mkdir /scripts/pre-exec.d && \
    mkdir /scripts/pre-init.d && \
    chmod -R 755 /scripts

EXPOSE 3306

VOLUME ["/var/lib/mysql"]

ENTRYPOINT ["/scripts/install.sh"]
