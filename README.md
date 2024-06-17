# Docker-Fundamentals

`https://docs.docker.com/`
`https://aws.amazon.com/docker/`

This repo will cover the concepts of Docker.

Docker is an open-source platform designed to automate the deployment, scaling, and management of applications using containerization. Containers are lightweight, stand-alone, and executable software packages that include everything needed to run an application, such as the code, runtime, system tools, libraries, and settings.

**Key Features of Docker:**

_Containerization_: Docker allows you to package an application and its dependencies into a standardized unit called a container. This ensures consistency across multiple development, testing, and production environments.

_Isolation_: Each container operates in isolation from others, with its own file system, processes, and network stack. This ensures that applications do not interfere with each other.

_Lightweight_: Containers share the host system's kernel, making them much more efficient than traditional virtual machines, which require a full OS instance for each application.

_Portability_: Docker containers can run on any system that supports Docker, making it easy to move applications between different environments, such as from a developer's laptop to a production server.

_Efficiency_: Because containers share the same OS kernel, they can start up much faster and use fewer resources compared to virtual machines.

**Core Components of Docker:**

_Docker Engine_: The core part of the Docker system, which creates and runs Docker containers. It includes:

  Docker Daemon: A background service that manages Docker containers, images, networks, and storage volumes.
  Docker CLI: A command-line interface that allows users to interact with Docker Daemon to create, manage, and monitor containers.

_Docker Images_: Read-only templates used to create containers. Images are built from a Dockerfile, which contains a series of instructions to set up the environment within the container.

_Docker Containers_: Instances of Docker images that run applications. They are isolated environments where the application code and dependencies are executed.

_Docker Hub_: A cloud-based repository where Docker users can store and share Docker images.

**Useful Commands**

`sudo service docker <start/stop>`

`docker --help`

`docker --version`

`docker ps`    list running containers

`docker info`

`docker pull <image-name>`

`sudo usermod -a -G docker test-user` adding user to the docker group.

`docker images`

- `docker images -q` will get image-id

`docker run <image-name>`

`docker rmi --help`                   removes 1 or more images

`docker stats`

`docker system df`

`docker system prune` be cautious while using this command 
