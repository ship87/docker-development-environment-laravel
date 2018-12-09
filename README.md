# Docker development environment Laravel

Using Docker in Laravel development for Ubuntu

PHP-FPM + Xdebug + Nginx  
PHP 7.0, 7.1, 7.2


# Docker
docker-compose up -d\
docker-compose up -d --force-recreate --no-deps --build\
docker system prune --all --volumes

docker network inspect bridge - find IP to connect for remote database

docker logs -f --details CONTAINER

docker logs [OPTIONS] CONTAINER
--details				Show extra details provided to logs\
--follow , -f			Follow log output\
--since					Show logs since timestamp (e.g. 2013-01-02T13:23:37) or relative (e.g. 42m for 42 minutes)\
--tail	all				Number of lines to show from the end of the logs\
--timestamps , -t		Show timestamps\
--until					API 1.35+\

sudo service docker restart

# Laravel

sudo chmod -R 777 bootstrap\
sudo chmod -R 777 storage

# Xdebug

Xdebug ports
 
PHP 7.0 - 8088\
PHP 7.1 - 8089\
PHP 7.2 - 8090

ls /sys/class/net - find network interface

eth0 - network interface

sudo ip addr add 10.254.254.254/24 brd + dev eth0 label eth0:1 - enable Xdebug
