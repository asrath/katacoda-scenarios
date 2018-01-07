## Open a shell against a container

We can open a shell against a container by running the shell executable.

For example: `docker run -ti --rm busybox sh`{{execute}}. `-t` and `-i` options instruct
docker to allocate a pseudo tty and run in interactive mode, these to options are required to be able to interact with the shell.
The `--rm` option removes the container when it stops. Once we write `exit`{{execute}} inside the container shell the container
will stop and then immediately be removed.

## Open a shell against an already running container

We also can open a shell inside against a running container. To do so we will use `docker exec`.

We will open a shell against our `background_ping` container. `docker exec -ti background_ping sh`{{execute}}.

**Note:** Here we are using `sh` shell because `busybox` image doesn't have bash installed. But we could use whatever 
shell is installed in the image.