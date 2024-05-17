# Docker Practice Exercises

Welcome to the Docker Practice Exercises repository! This repository contains a series of Jira tickets designed to help you practice and improve your Docker skills. Each ticket represents a specific exercise, guiding you through different aspects of Docker, from creating Dockerfiles to managing multi-container applications with Docker Compose.

## Table of Contents

- [Introduction](#introduction)
- [Exercises](#exercises)
  - [Ticket 1: Create a Dockerfile for a Simple Web Application](#ticket-1-create-a-dockerfile-for-a-simple-web-application)
  - [Ticket 2: Build and Run a Docker Image Locally](#ticket-2-build-and-run-a-docker-image-locally)
  - [Ticket 3: Push Docker Image to Docker Hub](#ticket-3-push-docker-image-to-docker-hub)
  - [Ticket 4: Create a Docker Compose File for Multi-Container Application](#ticket-4-create-a-docker-compose-file-for-multi-container-application)
  - [Ticket 5: Use Docker Volumes for Persistent Storage](#ticket-5-use-docker-volumes-for-persistent-storage)
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Docker is a powerful platform for developing, shipping, and running applications inside containers. This repository provides hands-on exercises to help you get started with Docker, covering basic to intermediate tasks. Each exercise is structured as a Jira ticket, detailing the objectives, steps, and acceptance criteria.

## Exercises

### Ticket 1: Create a Dockerfile for a Simple Web Application

**Summary**: Create a Dockerfile for a simple web application.

**Description**:
- Create a Dockerfile that sets up a simple web application.
- Use a base image like `node:alpine`.
- Copy the application source code into the container.
- Install necessary dependencies and run the application.

**Acceptance Criteria**:
- A Dockerfile is created in the root directory of the project.
- The Dockerfile uses `node:alpine` as the base image.
- The application source code is copied into the container.
- Dependencies are installed and the application starts successfully when the container is run.

### Ticket 2: Build and Run a Docker Image Locally

**Summary**: Build and run a Docker image locally.

**Description**:
- Use the Dockerfile created in the previous ticket.
- Build the Docker image using `docker build`.
- Run the Docker image using `docker run`.
- Ensure the web application is accessible locally.

**Acceptance Criteria**:
- The Docker image is built successfully without errors.
- The Docker container runs successfully and the application is accessible at `http://localhost`.

### Ticket 3: Push Docker Image to Docker Hub

**Summary**: Push Docker image to Docker Hub.

**Description**:
- Tag the locally built Docker image appropriately.
- Push the tagged Docker image to a Docker Hub repository.
- Ensure the image is accessible from Docker Hub.

**Acceptance Criteria**:
- The Docker image is tagged and pushed to Docker Hub.
- The image is visible in the specified Docker Hub repository.

### Ticket 4: Create a Docker Compose File for Multi-Container Application

**Summary**: Create a Docker Compose file for a multi-container application.

**Description**:
- Create a `docker-compose.yml` file to define a multi-container application.
- Include at least two services: a web application and a database (e.g., MySQL).
- Configure the services to communicate with each other.

**Acceptance Criteria**:
- A `docker-compose.yml` file is created in the root directory.
- The file defines at least two services (web app and database).
- The services can start and communicate with each other successfully.

### Ticket 5: Use Docker Volumes for Persistent Storage

**Summary**: Use Docker volumes for persistent storage.

**Description**:
- Update the Docker Compose file to use Docker volumes for data persistence.
- Mount a volume to the database service to ensure data is not lost when the container stops.
- Verify that data persists across container restarts.

**Acceptance Criteria**:
- The `docker-compose.yml` file is updated to include Docker volumes.
- The database service uses a volume for its data directory.
- Data persists across container restarts, as verified by creating data, stopping the container, and then starting it again.

## Getting Started

To get started with these exercises, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/docker-practice-exercises.git
   cd docker-practice-exercises

2. Follow the instructions in each ticket to complete the exercises. Start with Ticket 1 and work your way through to Ticket 5.

## Contributing

We welcome contributions to enhance these exercises or add new ones! If you have an idea for an improvement or a new exercise, please open an issue or submit a pull request.