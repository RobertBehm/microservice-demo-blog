
## Overview

This project demonstrates a basic microservice architecture where multiple services work together, each running in its own Docker container. The application is containerized using Docker and orchestrated using Kubernetes, which provides powerful tools for managing and scaling applications in production environments.

## Features

- **Microservice Architecture**: The application is divided into multiple services, each responsible for a specific piece of functionality.
- **Dockerized Services**: Each service runs in its own Docker container, ensuring consistency and portability across different environments.
- **Kubernetes Orchestration**: The application is deployed and managed using Kubernetes, which automates deployment, scaling, and management of containerized applications.

## Project Structure

- **`/client`**: Contains the React application.
- **`/posts`**: Contains the Posts service built with Express.js.
- **`/moderation`**: Contains the Moderation service built with Express.js.
- **`/query`**: Contains the Query service built with Express.js.
- **`/event-bus`**: Contains the Event Bus service that facilitates communication between services.
- **`/infra/k8s`**: Contains Kubernetes manifests for deploying the services.
- **`Dockerfile`**: A Dockerfile for each service, defining the environment and commands needed to run the service inside a Docker container.
- **`skaffold.yaml`**: Configuration file for Skaffold, a tool that facilitates continuous development for Kubernetes applications.

## Prerequisites

To run this demo, you'll need the following tools installed:

- **Docker**: To build and run Docker containers.
- **Kubernetes**: To orchestrate the containers and manage the application lifecycle.
- **kubectl**: The Kubernetes command-line tool to interact with your Kubernetes cluster.
- **Skaffold** (optional): For easier management of the continuous development workflow with Kubernetes.
