# Golang Cross Compile Docker Image

This repo contains a Dockerfile for building an image which is used to cross compile golang. It includes the MinGW compiler for windows, and an OSX SDK.

This image is available from https://hub.docker.com/r/level/golang-cross.

## Building

```shell
$ docker build -t levelio/golang-cross:x.y.z .
```

## Usage

Open a bash shell and run commands:
```shell
$ docker run -it levelio/golang-cross:latest bash
```

Or use it as a base image to build your own:
```docker
FROM levelio/golang-cross:latest

# Write your own Dockerfile
```
