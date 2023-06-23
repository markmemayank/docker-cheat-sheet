# Docker Cheat Sheet

## IMAGES

Docker images are a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

#### Build an Image from a Dockerfile
```docker build -t <image_name>```

#### Build an Image from a Dockerfile without the cache
```docker build -t <image_name> . –no-cache```

#### List local images
```docker images```

#### Delete an Image
```docker rmi <image_name>```

#### Remove all unused images
```docker image prune```

## DOCKER HUB

Docker Hub is a service provided by Docker for finding and sharing container images with your team. Learn more and find images
at https://hub.docker.com

#### Login into Docker
```docker login -u <username>```

#### Publish an image to Docker Hub
```docker push <username>/<image_name>```

#### Search Hub for an image
```docker search <image_name>```

#### Pull an image from a Docker Hub
```docker pull <image_name>```

## GENERAL COMMANDS

#### Start the docker daemon
```docker -d```

#### Get help with Docker. Can also use –help on all subcommands
```docker --help```

#### Display system-wide information
```docker info```
