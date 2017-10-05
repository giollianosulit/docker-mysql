# Simple Docker MariaDB - MySQL Container

This is a simple MariaDB MySQL Docker container using Docker Compose.
To access it use: LOCAL_IP:3306 / MACHINE_IP:3306 and make sure the username / passwords are set correctly in docker-compose.yml.

## System Requirements
Docker - https://www.docker.com/get-docker
Composer file is built using version 2.

## Notes
MySQL will also be mapped directly to the repository in the folder:

```
mysql
```

which is persistently mapped to:

```
/var/lib/mysql
```

## Getting it up and running
Here are a few basic commands to get started

### Starting the docker container (please update the settings first mentioned above)
```
docker-compose up -d
```

### Stopping Container
I recommend using STOP instead of DOWN to avoid losing any files.

* Note - Command might be different on Windows (I'm personally using OSX)
```
docker stop $(docker ps -a -q)
```