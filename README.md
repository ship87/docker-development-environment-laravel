# docker_development_environment_laravel

Using Docker in Laravel evelopment


docker-compose up -d

docker-compose up -d --force-recreate --no-deps --build

docker system prune --all --volumes


docker logs -f --details CONTAINER

docker logs [OPTIONS] CONTAINER

--details				Show extra details provided to logs

--follow , -f			Follow log output

--since					Show logs since timestamp (e.g. 2013-01-02T13:23:37) or relative (e.g. 42m for 42 minutes)
--tail	all				Number of lines to show from the end of the logs

--timestamps , -t		Show timestamps

--until					API 1.35+



sudo service docker restart

sudo chmod -R 777 bootstrap

sudo chmod -R 777 storage
