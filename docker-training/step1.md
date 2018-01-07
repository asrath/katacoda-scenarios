Lets get your hands dirty

## docker run

To run a container we will use **docker run** command. **docker run** tries to find a local image to run, if the specified image doesn't exist
**docker** will try to download it from https://hub.docker.com.

The docker run syntax is `docker run [options] <image> [command]`

We will run a ping command using a [busybox](https://en.wikipedia.org/wiki/BusyBox) image.

`docker run busybox ping 127.0.0.1`{{execute}}

To stop the process press `Ctrl+C` ``{{execute interrupt}}