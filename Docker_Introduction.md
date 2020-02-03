# Docker Introduction

- Docker is a utility software. It is an Open-Source project that automates the deployment of software application inside containers by providing an additional Layer of abstraction and automataion of OS-level virtualization on linux.
- Compatible with **Linux** Operating System. So if working on Windows you can pull the box through Vagrant and work on the virtualized environment.

## Terminologies

- Image- The blueprint of our appplication which form the basis of containers. You can take it as a class which is a blueprint of object. Coming ahead, we will see that image will be stored on hard disk and container will run on RAM.
- Container- Created from Docker images and run the actual application. We create a container using `docker run`. There is a specific limit upto which we can make container as it can create a overflow situation in RAM and thus can make processes waiting. 

## Commands to run Docker

- `docker pull`:- Pulls the image from docker hub. Generally used when we have to pull multiple images.
- `docker ps`:- lists the current running containers.
- `docker ps -a`:- lists the executed conatiners.
- `docker images`:- lists the images which are being pulled.
- `docker run **image name/container id** -it`:- runs the container in interactive mode.
- `docker run **image name/container id** -d`:- runs the conatiner in the backend.
- `docker run **image name/conatiner id**`:- runs the container and exits after execution.
- `docker load`:- Loads the image other than docker hub or from a hard disk or pen drive.
- `docker push`:- 
- `docker ssh`:-

## Docker States

- start
- suspend
- exited
