# CodeAlpha Web Server using Docker

## Overview

This project is a Docker-based web server developed as part of the CodeAlpha DevOps Internship. It demonstrates how to containerize and deploy a simple web server using Docker and NGINX.

## Technologies Used

* Docker
* NGINX
* HTML
* Git and GitHub

## Project Structure

```text
CodeAlpha_WebServer/
├── Dockerfile
├── index.html
└── README.md
```

## How It Works

1. The `Dockerfile` uses the NGINX image as the base image.
2. The `index.html` file contains the web page content.
3. Docker builds an image from the Dockerfile.
4. A container is created from the Docker image.
5. NGINX serves the HTML page inside the container.
6. Port `8080` on the host is mapped to port `80` inside the container.

## Docker Commands Used

### Build the Docker image

```bash
docker build -t codealpha-webserver .
```

### Run the container

```bash
docker run -d -p 8080:80 --name codealpha-webserver-container codealpha-webserver
```

### Check running containers

```bash
docker ps
```

### Stop the container

```bash
docker stop codealpha-webserver-container
```

### Start the container again

```bash
docker start codealpha-webserver-container
```

### View container logs

```bash
docker logs codealpha-webserver-container
```

### Monitor container resources

```bash
docker stats codealpha-webserver-container
```

## Access the Web Server

After starting the container, open:

```text
http://localhost:8080
```

The NGINX web server displays the custom HTML page.

## Learning Outcomes

This project provides practical experience with:

* Docker containerization
* Docker images and containers
* NGINX web server deployment
* Port mapping
* Container lifecycle management
* Container monitoring and troubleshooting
* Git and GitHub

## Internship Task

**CodeAlpha DevOps Internship — Task 4: Web Server using Docker**
