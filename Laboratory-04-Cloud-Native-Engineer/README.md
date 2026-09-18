# Laboratory 04 - The Cloud-Native Engineer

## Mission Overview

In this laboratory activity, I learned the basics of cloud-native engineering and containerization. I compared traditional Virtual Machines (VMs) with Docker containers and used the KillerCoda Playground to practice Docker commands. I also deployed an Nginx web server inside a Docker container and managed its lifecycle by running, stopping, and removing the container.

## Objectives

* Differentiate between Virtual Machines and Containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Execute fundamental Docker CLI commands.
* Pull and run an Nginx container.
* Map a host port to a container port.
* Manage the lifecycle of a Docker container.
* Document container operations using Markdown.
* Maintain an organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Checkpoint 3 - Verify Docker

```bash
docker --version
```

```bash
docker info
```

### Checkpoint 4 - Deploy Nginx

```bash
docker pull nginx
```

```bash
docker run -d -p 8080:80 --name nginx nginx
```

```bash
curl http://localhost:8080
```

### Checkpoint 5 - Container Lifecycle

```bash
docker ps
```

```bash
docker stop nginx
```

```bash
docker ps
```

```bash
docker ps -a
```

```bash
docker rm nginx
```

```bash
docker ps -a
```

## Skills Learned

Through this activity, I learned how Docker containers work and how they differ from traditional Virtual Machines. I learned how to pull Docker images, create and run containers, map ports, and check whether a container is running. I also practiced stopping and removing containers and documenting technical procedures using Markdown and GitHub.

## Challenges Encountered

One challenge I encountered was identifying the correct Docker container name when managing the container lifecycle. I initially tried to stop a container using the name `nginx`, but there was no container with that name because the container was no longer present. I resolved the issue by checking the Docker container list and recreating the Nginx container with a specific name. This helped me understand the importance of checking container status and names before performing Docker management commands.

