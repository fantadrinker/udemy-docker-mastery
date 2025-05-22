
```
docker container run --detach -p 80:80 --name nginx1 nginx
docker container run --detach -p 8080:80 --name httpd1 httpd
docker container run --detach -p 3306:3306 --env "MYSQL_RANDOM_ROOT_PASSWORD=yes" --name mysql1 mysql

docker container logs mysql1 | grep PASSWORD
```
