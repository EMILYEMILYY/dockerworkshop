

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
