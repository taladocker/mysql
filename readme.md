## Introduction
This is a Dockerfile to build a container image for mysql

## Git repository
The source files for this project can be found here: https://github.com/taladocker/mysql

## Pulling from Docker Hub
Pull the image from docker hub rather than downloading the git repo. This prevents you having to build the image on every docker host:

```
docker pull tala/mysql
```

## Running
To simply run the container:

```
docker run --name talaria-mysql -v /my/own/datadir:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=my-secret-pw -d tala/mysql:dev
```
