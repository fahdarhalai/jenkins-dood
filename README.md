# Jenkins Docker Outside Of Docker

This is a Jenkins container that binds docker socket from host machine.

If you use named volumes to persist Jenkins home, create a docker volume using:
```shell
docker volume create docker_jenkins_home
```
otherwise, use bind mounts.

Build the image and run the container using:
```shell
docker compose up -d
```