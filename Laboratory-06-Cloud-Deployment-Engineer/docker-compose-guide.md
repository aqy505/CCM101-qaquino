# Docker Compose Guide — Nextcloud + MariaDB Deployment

This document explains the `docker-compose.yml` file used to deploy the
two-tier Nextcloud stack.

## What does the `services:` block do?
`services:` is the top-level key in the Compose file that defines every
container Compose should manage. Each entry under it `database` and `app`
in this file names one service, and its nested configuration (`image`,
`environment`, `ports`) tells Compose what image to run and how to configure
that container.

## How did the Nextcloud app container find the database container?
Through the environment variable `MYSQL_HOST=database`. When Docker Compose
starts a stack, it automatically creates a shared network for all services
defined in the file and registers each service's name as a resolvable DNS
hostname on that network. Because the database service is named `database`,
the app container can reach it simply by connecting to the hostname
`database` Compose's internal DNS resolves that name to the database
container's IP address. No manual IP configuration or linking is needed.

## What is the difference between `docker run` and `docker-compose up -d`?
`docker run` starts a single container at a time, and every configuration
option (image, ports, environment variables, network) has to be typed out as
flags each time you run it. `docker-compose up -d` instead reads a single
declarative YAML file describing the entire multi-container stack and starts
(or recreates) every service in it together, automatically wiring up
networking between them. This is the core idea of Infrastructure as Code —
the desired state of the whole system is written down once, version-
controlled, and reproduced consistently, rather than rebuilt from a sequence
of manual commands.