#FROM php:fpm-alpine
FROM php:7.3.4-fpm-alpine3.9
MAINTAINER Sonny Yu <sonnyyuirm@gmail.com>
RUN apk add --upgrade --no-cache tzdata \
     && rm -rf /var/cache/apk/* /tmp/*
ENV TZ=America/Los_Angeles
RUN docker-php-ext-install mysqli
ADD ./www.tar.gz  /srv