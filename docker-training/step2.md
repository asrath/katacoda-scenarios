## Containers

A container is a running image instance. In docker each container usually runs a single process.

In order to list containers we will use `docker ps`{{execute "HOST1"}} for active containers.
This command will be executed in another terminal to show the currently running container.

Then execute `docker ps -a`{{execute interrupt}} to show all containers. If you want to stop a running
container in foreground use `Ctrl+C`.

## Images

In order to list images we use `docker images`{{execute}}
