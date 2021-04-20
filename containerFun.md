docker container run --name nginx -d -p 80:80 nginx

docker container run --name apache -d -p 81:80 httpd

docker container run --name mysql -e MYSQL_ROOT_PASSWORD=password -d -p 3306:3306 mysql

docker container inspect mysql

docker container ls -a

docker container stop
docker container rm
docker container ls -a
