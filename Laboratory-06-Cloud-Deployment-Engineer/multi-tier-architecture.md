# Two-Tier Architecture

## What Is a Two-Tier Architecture?

A two-tier architecture is an application design that separates the application layer from the database layer. In this mission, Nextcloud handles the web application while MariaDB stores the application's data. Both run in separate Docker containers and communicate through Docker Compose.

## The Web/Application Tier

The web/application tier uses Nextcloud to provide the user interface for private cloud storage. It handles browser requests and allows users to manage their files through a web interface.

## The Database Tier

The database tier uses MariaDB to store persistent application data, such as user account information and file metadata. This data allows the application to maintain information between sessions.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage and troubleshoot. Each service can be configured, updated, and monitored separately instead of having both components packed into one container. It also makes it easier to scale individual services when necessary.
