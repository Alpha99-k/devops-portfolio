# Project 01: Dockerized ASP.NET Core Web Application

## Overview

This project demonstrates how to containerize and deploy an ASP.NET Core web application using Docker.

The application is packaged into a Docker image using a multi-stage Dockerfile and deployed as a running container using Docker Compose.

## Technologies Used

- ASP.NET Core (.NET 10)
- Docker
- Docker Compose
- Linux Containers
- Git and GitHub

## Architecture

The application follows a containerized deployment architecture:

1. ASP.NET Core provides the web application.
2. Docker builds the application into an image.
3. Docker Compose manages the container.
4. Port 8080 exposes the application to the host machine.

## Implementation

### 1. Application Development

Created an ASP.NET Core web application using Visual Studio.

### 2. Docker Configuration

Created a multi-stage Dockerfile to build and publish the application.

### 3. Containerization

Built the Docker image using:

```bash
docker compose build
```

### 4. Deployment

Started the application container using:

```bash
docker compose up -d
```

### 5. Verification

Verified the running container using:

```bash
docker ps
```

Application URL:

http://localhost:8080

## Docker Commands

| Command | Purpose |
|---|---|
| docker images | List available images |
| docker ps | List running containers |
| docker logs devops-webapp | View application logs |
| docker compose build | Build application image |
| docker compose up -d | Start application |
| docker compose down | Stop and remove container |

## Project Outcome

Successfully built a Docker image for an ASP.NET Core application and deployed it inside a running Docker container.

The application was accessible through the host machine using port 8080.

## Skills Demonstrated

- Docker image creation
- Multi-stage container builds
- ASP.NET Core deployment
- Container management
- Docker Compose
- Application troubleshooting
- Technical documentation

## Future Improvements

- Publish the Docker image to Docker Hub.
- Implement automated CI/CD using GitHub Actions.
- Add container health checks.
- Introduce application monitoring.
