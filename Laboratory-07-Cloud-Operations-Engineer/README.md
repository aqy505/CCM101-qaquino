# Laboratory 7: The Cloud Operations Engineer

## Mission Overview

This laboratory activity focuses on monitoring a Linux server and checking the performance of a containerized web application. I used Docker and Nginx to generate web traffic, check application logs, and monitor container resource usage.

## Objectives

* Check the server's RAM and disk storage.
* Deploy an Nginx web server using Docker.
* Generate HTTP requests and identify a missing page.
* Analyze application logs and monitor container metrics.
* Document the results using Markdown.

## Monitoring Commands Executed

* `free -h` – checked RAM usage.
* `df -h /` – checked root filesystem storage.
* `top` – monitored running processes and CPU activity.
* `docker run -d -p 8080:80 --name client-website nginx` – deployed the Nginx container.
* `curl http://localhost:8080` – tested website access.
* `curl http://localhost:8080/hidden-admin-page` – generated a 404 response.
* `docker logs client-website` – checked application logs.
* `docker stats` – monitored the container's CPU and memory usage.

## Skills Learned

* Monitoring Linux server resources.
* Deploying and testing a Docker container.
* Reading application logs to identify errors.
* Checking real-time container metrics.
* Writing technical reports using Markdown.
