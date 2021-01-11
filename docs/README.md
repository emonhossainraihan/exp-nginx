# Docker related command

## Run command inside docker

```
docker exec -it <CONTAINER> bash
```

## Copy nginx configuration file on local machine

```
docker run -p 8080:80 nginx -d
docker cp <CONTAINER_ID>:"etc/nginx/nginx.conf" "LOCAL-PATH"
```

## Install the editor on container

```
apt-get update
apt-get -y install vim
```
