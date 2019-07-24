<img src="https://raw.githubusercontent.com/KnowledgePending/Kitura-Docker/master/images/logo.png" width="500">

# [Simple Kitura Docker environment](https://github.com/KnowledgePending/Kitura-Docker)
[![Docker Pulls](https://img.shields.io/docker/pulls/bryankp/swift_kitura.svg)](https://hub.docker.com/r/bryankp/swift_kitura)
## Image details
* Ubuntu 18.04 Bionic
* Swift 5.0.2
* Kitura 0.0.16

## Option 1. Build Docker Image
* From within the directory of the Dockerfile execute the following command to build the image
```BASH
docker build -t swift_kitura .
```
* To run with bash and a shared volume
```BASH
docker run -v <host_path>:<container_path> -ti swift_kitura:latest bash
```
## Option 2. Pull image from Docker Hub
* Go to the repository page [bryankp/swift_kitura](https://hub.docker.com/r/bryankp/swift_kitura)
* Pull the latest image
```BASH
docker pull bryankp/swift_kitura:latest
```

* To run with bash and a shared volume
```BASH
docker run -v <host_path>:<container_path> -ti bryankp/swift_kitura:latest bash
```

### Further Details
* [Swift Official Docker Images](https://hub.docker.com/_/swift)
* For troubleshooting issues see the [Kitura Docs](https://www.kitura.io/index.html)


* To use the swift repl while running docker on macos the container needs to be run with the following flag --privileged
    * Example ```docker run --privileged -v $(pwd):/temp -ti kit:latest bash```
    * see https://github.com/apple/swift-docker/issues/9











