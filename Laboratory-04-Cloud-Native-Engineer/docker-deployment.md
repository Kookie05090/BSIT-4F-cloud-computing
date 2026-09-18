## Checkpoint 5 - The Container Lifecycle

### 1. List Running Containers

```bash
docker ps
```

This command lists all currently running Docker containers and shows information such as the container ID, image, status, ports, and container name.

### 2. Stop the Running Container

```bash
docker stop nginx
```

This command stops the running Nginx container.

### 3. Verify the Container is Stopped

```bash
docker ps
```

This command verifies that the Nginx container is no longer running because stopped containers do not appear in the list.

### 4. Check All Containers

```bash
docker ps -a
```

This command displays all Docker containers, including containers that have been stopped.

### 5. Remove the Container Completely

```bash
docker rm nginx
```

This command removes the stopped Nginx container completely from the Docker environment.

### 6. Verify the Container Was Removed

```bash
docker ps -a
```

This command verifies that the Nginx container has been completely removed and no longer appears in the container list.

### Screenshot Evidence

The screenshot below shows the execution of the container lifecycle commands:

`container-lifecycle.png`

