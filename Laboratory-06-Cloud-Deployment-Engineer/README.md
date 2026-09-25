
# Laboratory 06 – Cloud Deployment Engineer

## Mission Overview

This laboratory focuses on deploying a multi-container cloud storage application using Docker Compose. Nextcloud serves as the web application, while MariaDB manages the database. Both services are configured through a YAML file and deployed together using a single command.

## Objectives

- Understand the concept of multi-tier architecture.
- Create and configure a docker-compose.yml file.
- Deploy Nextcloud and MariaDB using Docker Compose.
- Access the Nextcloud web interface through port 8080.
- Practice Infrastructure as Code (IaC).
- Document the deployment process using Markdown.

## Commands Executed

| Command | Purpose |
|---------|---------|
| `mkdir nextcloud-deployment` | Creates the project directory. |
| `cd nextcloud-deployment` | Moves into the project directory. |
| `nano docker-compose.yml` | Creates and edits the YAML configuration file. |
| `cat docker-compose.yml` | Displays the configuration file. |
| `docker compose up -d` | Deploys both containers in the background. |
| `docker compose ps` | Checks the status of the containers. |
| `docker compose down` | Stops and removes the containers. |


## Skills Learned

- Creating and editing YAML configuration files.
- Understanding the roles of application and database tiers.
- Deploying multiple containers using Docker Compose.
- Configuring environment variables for container communication.
- Accessing containerized applications through mapped ports.
- Managing the container lifecycle using Docker commands.
- Understanding the importance of Infrastructure as Code.