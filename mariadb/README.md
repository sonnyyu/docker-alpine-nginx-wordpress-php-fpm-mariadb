docker build -t docker-mariadb .

docker run -it --name docker-mariadb -p 3306:3306 -v $(pwd)/data:/var/lib/mysql -e MYSQL_DATABASE=wordpressdb -e MYSQL_ROOT_PASSWORD=password docker-mariadb

mysql -h127.0.0.1 -uroot -p

docker container prune -f

docker image prune -a -f

docker volume prune -f

docker network prune -f

docker system prune -f

sudo rm -rf /var/lib/docker/volumes/*

docker-mariadb      latest              bfa0b259e7c2        4 minutes ago       229MB
