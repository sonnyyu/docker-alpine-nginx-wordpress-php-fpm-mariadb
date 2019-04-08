FROM nginx:1.15.10-alpine
MAINTAINER Sonny Yu <sonnyyuirm@gmail.com>
RUN  apk add --upgrade --no-cache tzdata \
     && rm -rf /var/cache/apk/* /tmp/*
ENV  TZ=America/Los_Angeles
COPY ./default.conf /etc/nginx/conf.d/default.conf