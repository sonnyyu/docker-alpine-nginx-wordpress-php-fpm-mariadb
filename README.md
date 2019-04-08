# docker-nginx-phpfpm-alpine

Basic Docker setup for running Nginx + PHP-FPM on Alpine Linux.

docker-compose down \
docker container prune -f \
docker image prune -a -f \
docker volume prune -f \
docker network prune -f \
docker system prune -f \
sudo rm -rf /var/lib/docker/volumes/*

docker-compose config \
docker-compose build \
docker-compose up -d

