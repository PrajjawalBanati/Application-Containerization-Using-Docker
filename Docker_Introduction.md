# What is Docker? (build,ship and run)

- Docker is a tool to create,run and deploy applications using containers. It allows developers to packge the application with all types of dependencies and libraries and ship it all as one package
-It is an Open-Source project that automates the deployment of software application inside containers by providing an additional Layer of abstraction and automataion of OS-level virtualization on linux.
- Compatible with **Linux** Operating System. So if working on Windows you can pull the box through Vagrant and work on the virtualized environment.
- In ensures that your application works seamlessly in any environment; be it Development, Test or Production.

# Who uses Docker in the Lifecycle of a Project ?

- **Developer**
	- It helps developer to build great software and makes him easy to deploy his unit package as a docker image which can run on system administrators.
	
- **Sysadmin**
	- When the unit package is deployed by the developer it needs to be checked in the prod,stage and test environment. Now unlike before the administrator will recieve a docker image which will contain all the dependencies and libraries which will be needed to run the product so docker (present in sysadmin system) will download all the files and libraries which are present in the docker image and then the product will be tested without any missing dependency error.
	
	![img](https://github.com/PrajjawalBanati/Application-Containerization-Using-Docker/blob/master/Outputs/Docker_Introduction(Step-1).JPG)
	
# How Docker works?(In a Nutshell)

- First the developers make a docker file which is used to build docker image. 
- Now when docker image is created then it could be run on different containers as you want.
- The created images can be uploaded on Docker Hub from where the image can pulled and built in a container.
	
	![img](https://github.com/PrajjawalBanati/Application-Containerization-Using-Docker/blob/master/Outputs/Docker_Introduction(Step-2).JPG)

# What is an Image?

- The blueprint of our appplication which form the basis of containers. You can take it as a class which is a blueprint of object. 
- In other words it is text file(Can be said as Docker File) which contains pre-written commands which make multiple layers of the system.
- For each instruction in the dockerfile a layer is created and it is placed on top of the previous layer.
- Image can be said as read-only filesystem means the system created is not writable at all. When this image is turned into a container the Docker engine takes the image and adds a read-write filesystem on top.

	![img](https://github.com/PrajjawalBanati/Application-Containerization-Using-Docker/blob/master/Outputs/Docker_Introduction(Step-3).JPG)

## Hello World In Docker
- **Installation Of Docker:-**
	- For linux operating systems first run the update command.<br>
		- `sudo apt-get update`
			![img_0](https://github.com/PrajjawalBanati/Application-Containerization-Using-Docker/blob/master/Outputs/Docker_Install(Step-1).JPG)
	- Then install docker.io file by using apt installer.<br>
		- `sudo apt-install docker.io`
			![img_1](https://github.com/PrajjawalBanati/Application-Containerization-Using-Docker/blob/master/Outputs/Docker_Install(Step-2).JPG)
- **Running Hello-World Image:-**
	- Then search hello world image file in the docker registry by the following command.<br>
		- `docker search hello`
			![img_3](https://github.com/PrajjawalBanati/Application-Containerization-Using-Docker/blob/master/Outputs/Docker_Install(Step-4).JPG)
	- Then pull the image from the docker registry using the following command.<br>
		- `docker pull hello-world`
			![img_2](https://github.com/PrajjawalBanati/Application-Containerization-Using-Docker/blob/master/Outputs/Docker_Install(Step-5).JPG)
	- After the image gets pulled you now can run the image in the container by using the following command.<br>
		- `docker run hello-world`
			![img_4](https://github.com/PrajjawalBanati/Application-Containerization-Using-Docker/blob/master/Outputs/Docker_Install(Step-3).JPG)

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
