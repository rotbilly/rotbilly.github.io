Official Docker Hub Link [https://hub.docker.com/_/mariadb]

- Install & Start
```sh
docker run --name sna_my -v ~/docker/volumes/mysql:/var/lib/mysql -p 3306:3306 -e MARIADB_ROOT_PASSWORD=mariadbpw -d mariadb:latest

docker start sna_my || docker run --name sna_my -v ~/docker/volumes/mysql:/var/lib/mysql -p 3306:3306 -e MARIADB_ROOT_PASSWORD=mariadbpw -d mariadb:latest

```

- Stop & Start
```sh
docker stop sna_my
docker stop ${container_name}

docker start sna_my
docker start ${container_name}
```

- Backup & Recovery
```sh


```