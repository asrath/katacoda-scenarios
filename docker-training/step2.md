## Containers

A [container](https://docs.docker.com/glossary/?term=container) is a runtime instance
of a [docker image](https://docs.docker.com/glossary/?term=image).
In docker each container usually runs a single process.

In order to list all containers `docker ps -a`{{execute interrupt}} to show all containers.
If you want to stop a running container in foreground use `Ctrl+C`.

Execute `docker run -d --name background_ping busybox ping 127.0.0.1`{{execute}}. Note that we added the `-d` option to
run the container in background and `--name` to set the container name (by default is random).

In order to list running containers we will use `docker ps`{{execute}}.

## Images

[Docker images](https://docs.docker.com/glossary/?term=image) are the basis of [containers](https://docs.docker.com/glossary/?term=container).
An Image is an ordered collection of root filesystem changes and the corresponding execution parameters for use within a container runtime. An image typically contains a union of layered filesystems stacked on top of each other. An image does not have state and it never changes.

In order to list images we use `docker images`{{execute}}
