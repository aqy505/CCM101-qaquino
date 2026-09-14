# Docker Deployment

## The Container Lifecycle

### 1. List Running Containers

```bash
docker ps
```

This command displays all Docker containers that are currently running.

### 2. Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container named `nginx-server`.

### 3. Verify It Is Stopped

```bash
docker ps -a
```

This command displays all containers, including stopped ones, to verify that the Nginx container has stopped.

### 4. Remove the Container Completely

```bash
docker rm nginx-server
```

This command permanently removes the stopped `nginx-server` container from Docker.