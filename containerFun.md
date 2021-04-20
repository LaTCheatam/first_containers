docker container run --name nginx -d -p 80:80 nginx

docker container run --name apache -d -p 81:80 httpd

docker container run --name mysql -e MYSQL_ROOT_PASSWORD=password -d -p 3306:3306 mysql

docker container inspect mysql

docker container ls -a

docker container stop
docker container rm
docker container ls -a

Phase 1 ************************************

docker container run -it --name web nginx zsh

exit #exit and stop shell

docker container start web # to start container

docker container exec -it web bash #starts bash and puts in root of container

exit # exit and leave container running

docker container run --name ubuntu -d -t ubuntu

docker exec -i ubuntu bash

apt-get update
apt-get install -y curl
curl parrot.live
exit
docker container ls

docker container run -it --name notliketheother ubuntu bash

docker container run --name characters -d -t alpine
docker exec -i characters sh

bin/sh -c "while :; do wget -qO- https://swapi.dev/api/people/?search=r2; printf '\n'; sleep 5s; done"

## to run in background append command with container run. example: docker container run --name characters -d -t alpine bin/sh -c "while :; do wget -qO- https://swapi.dev/api/people/?search=r2; printf '\n'; sleep 5s; done"