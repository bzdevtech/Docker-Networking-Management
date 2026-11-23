
# Docker Networking Management

## Overview

This repository contains two practical activities designed to explore Docker networking and understand how containers communicate with one another.

## Activity 1 — Networking with an Existing Docker Image

Reuse the Nginx-based static website image created during **Lab 2 — Docker Image Management** to explore Docker networking.

### Getting the Docker Image

You can choose either of the following options.

**Option 1 — Use the prebuilt image from Docker Hub**

The image has already been built and published on Docker Hub.

- **Docker Hub Repository:** https://hub.docker.com/r/tsebaze/static_site_image
- **Image Tag:** `labs2-v1`
- **Full Image Reference:** `tsebaze/static_site_image:labs2-v1`

**Option 2 — Build the image from the source code**

You can access the source code and Dockerfile on GitHub and build the image locally.

- **GitHub Repository:** https://github.com/bzdevtech/Docker-Image-Management

### Exercise 1: Containers on the Default Bridge Network

- Create two containers named `web_app_1` and `web_app_2` using the existing Docker image.
- Do not explicitly specify a network or publish any ports.
- Inspect both containers and identify their network configuration and IP addresses.
- Enter `web_app_1` and test communication with `web_app_2` using its IP address.

### Exercise 2: Creating a Custom Bridge Network

- Create a custom Docker bridge network named `network-app-3`.
- Create a third container named `web_app_3` and connect it to the custom network.
- Inspect `web_app_3` to identify its network configuration and IP address.
- From `web_app_1`, test communication with `web_app_3` using its IP address.
- Observe and compare the communication behaviour of containers connected to different networks.

### Exercise 3: Exploring Host Networking

- Create a fourth container named `web_app_4` using host networking.
- Inspect the container's network configuration.
- Examine the IP address information provided by Docker and investigate how host networking works in the current environment.

### Bonus: Container Management

- Explore commands for displaying container IDs.
- Practise stopping running containers.
- Practise removing containers, including stopped containers.

## Activity 2 — Networking with Ubuntu

Use the official Ubuntu image to explore communication between containers connected to a custom Docker bridge network.

### Exercise 1: Creating a Bridge Network

- Create a custom Docker network using the bridge driver.

### Exercise 2: Creating Ubuntu Containers

- Create two Ubuntu containers and connect both to the network created for this activity.

### Exercise 3: Preparing the Containers

- Install the `ping` utility in the Ubuntu containers when necessary.
- Identify the IP addresses of both containers.

### Exercise 4: Testing Container Connectivity

- Test communication between the two containers using their IP addresses.
- Test communication between the two containers using their names.
- Observe the results and compare the two methods of communication.

## Learning Objectives

By completing these activities, learners will be able to:

- Understand the default bridge network and custom bridge networks.
- Explore host networking and its behaviour in the current Docker environment.
- Inspect Docker containers and identify their network configurations and IP addresses.
- Test communication between containers using IP addresses and container names.
- Understand how Docker network configuration affects container connectivity.
- Practise essential commands for managing containers.
