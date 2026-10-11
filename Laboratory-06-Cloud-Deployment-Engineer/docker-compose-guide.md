# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the containers that make up the application. In this project, it contains two services: `database`, which uses the MariaDB image, and `app`, which uses the Nextcloud image. Docker Compose uses these definitions to create and manage the application components together.

## How Does Nextcloud Find the Database?

The Nextcloud service uses the environment variable `MYSQL_HOST=database`. The value `database` matches the service name defined in the Compose file. Docker Compose provides service-name-based networking, allowing the application container to reach the database container through that name.

## Docker Run vs. Docker Compose Up -d

The `docker run` command is commonly used to create and start an individual container with options supplied on the command line. In contrast, `docker-compose up -d` reads the configuration from `docker-compose.yml` and starts the services defined there in the background. This makes a multi-container application easier to deploy consistently and manage as one project.

## Commands Used

- `mkdir nextcloud-deployment` — creates the project directory.
- `cd nextcloud-deployment` — enters the project directory.
- `nano docker-compose.yml` — creates or edits the Compose configuration.
- `docker-compose config` — validates and displays the resolved configuration.
- `docker-compose up -d` — starts the configured services in the background.
- `docker-compose ps` — displays the project's container status.
- `docker-compose logs --tail=50` — displays recent service logs.
- `docker-compose down` — stops and removes the project's containers and network.

## Infrastructure as Code

Infrastructure as Code (IaC) means defining infrastructure in configuration files rather than relying only on manual commands. The Compose YAML file documents the services, images, port mapping, and environment variables needed for this deployment. It can be reviewed, version-controlled, and reused for consistent deployments.
