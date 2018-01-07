## Stopping a container running in background

First list the containers all running containers with `docker ps`{{execute}}.

Then use `docker stop container_name [container_name...]` or `docker stop container_id [container_id...]`.

We will stop our `background_ping` container. `docker stop background_ping`{{execute}}.

## Removing containers

We can remove unused containers using `docker stop`.

First we list all containers `docker ps -a`{{execute}}.

Then we remove `background_ping` container `docker rm background_ping`{{execute}}.

We can also force remove running containers using `docker rm -f CONTAINER [CONTAINER...]`.