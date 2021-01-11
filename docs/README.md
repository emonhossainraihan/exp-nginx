# Docker related command

## Run command inside docker

```
docker exec -it <CONTAINER> bash
```

## Copy nginx configuration file on local machine

```
docker run -d -p 8080:80 nginx
docker cp <CONTAINER_ID>:"etc/nginx/nginx.conf" "LOCAL-PATH"
```

## Install the editor on container

```
apt-get update
apt-get -y install vim
```

[Editing files in a docker container](https://blog.softwaremill.com/editing-files-in-a-docker-container-f36d76b9613c)

## Running Nginx to restart

```
apt-get install systemd
systemctl restart nginx
```

OR

```
service nginx restart
```
