# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

This laboratory activity focuses on understanding cloud-native technology and the use of Docker containers. It covers the difference between Virtual Machines and Containers, setting up a Docker environment, deploying an Nginx web server, and managing the container lifecycle.

## Objectives

- Understand the differences between Virtual Machines and Containers.
- Learn the basic concepts of Docker and containers.
- Verify that Docker is installed and running.
- Pull and deploy an Nginx container.
- Run a web server using Docker.
- Learn how to start, check, stop, and remove containers.
- Practice basic Docker commands in a Linux environment.

## Docker Commands Executed

### Checkpoint 3 - Enter the Docker Playground

```bash
docker --version
```
Checks the installed version of Docker.

```bash
docker info
```
Displays information about the current Docker environment.

```bash
docker ps
```
Displays the currently running Docker containers.

### Checkpoint 4 - Deploy Your First Container

```bash
docker pull nginx
```
Downloads the official Nginx image.

```bash
docker run -d -p 8080:80 --name nginx-server nginx
```
Creates and runs the Nginx container in detached mode and maps port 8080 to port 80.

```bash
docker ps
```
Checks if the Nginx container is running.

```bash
curl http://localhost:8080
```
Sends an HTTP request to the local Nginx server to verify that it is working.

### Checkpoint 5 - The Container Lifecycle

```bash
docker ps
```
Lists all currently running containers.

```bash
docker stop nginx-server
```
Stops the running Nginx container.

```bash
docker ps -a
```
Displays all containers, including stopped containers.

```bash
docker rm nginx-server
```
Removes the stopped Nginx container completely.

## Skills Learned

- Using basic Docker commands.
- Pulling Docker images from Docker Hub.
- Creating and running Docker containers.
- Mapping ports between the host and a container.
- Testing a web server using `curl`.
- Managing the lifecycle of Docker containers.
- Using Docker in a Linux environment.

## Challenges Encountered

One challenge was becoming familiar with the different Docker commands and understanding what each command does. I also had to understand how port mapping works when connecting port 8080 of the host to port 80 of the Nginx container. After following the commands step by step and checking their outputs, I was able to understand the basic process of deploying and managing containers.