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

docker-mariadb      latest                a8d8b1b71f4c        5 minutes ago       230MB \
docker-phpfpm       latest                b48230d70ea2        6 minutes ago       125MB \
docker-nginx        latest                cda48f3eff6f        6 minutes ago       20.1MB


