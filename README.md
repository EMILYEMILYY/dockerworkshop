# dockerfiles-centos-user-adderable
Centos7, It support base user creation and password setting.

# Building & Running

Copy the sources to your docker host and build the container, and to run.
```
	docker build --rm -t emilyemilyy/nginx .
	docker run -it --name n1 emilyemilyy/nginx
```
Get the port that the container is listening on:

```
# docker ps
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES
ad2ad96e4b2f        emilyemilyy/nginx      "/bin/bash"         7 seconds ago       Up 6 seconds                            c1
```

To test, ("nowage" is username. )
```
	su - nowage
```
To Rollback
```
    docker rm c1 -f
    docker rmi nowage/centos7
```
