
docker -v

docker container run alpine echo "Hello World"

docker image ls
docker container ls
docker container ls -a
docker container rm bold_bardeen

docker container run --name centos centos
docker container run --name centos -p 80:80 centos

ping -c 5 127.0.0.1

docker container run centos ping -c 5 127.0.0.1