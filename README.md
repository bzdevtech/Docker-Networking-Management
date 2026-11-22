
# Docker Networking Management

## Overview

This repository contains two practical activities designed to explore Docker networking and understand how containers communicate with one another.



### Activity 1 — Networking with an Existing Docker Image

Reuse the Nginx image created during [Lab 2 — Docker Image Management](https://github.com/bzdevtech/Docker-Image-Management) to explore Docker networking.

#### Exercise 1: Containers on the Default Bridge Network
- Create two containers named `web_app_1` and `web_app_2` using the existing Docker image.
- Do not explicitly specify a network or publish any ports.
- Inspect both containers and identify their network configuration and IP addresses.
- Enter `web_app_1` and test communication with `web_app_2` using its IP address.

#### Exercise 2: Creating a Custom Bridge Network
- Create a custom Docker bridge network named `network-app-3`.
- Create a third container named `web_app_3` and connect it to the custom network.
- Inspect `web_app_3` to identify its network configuration and IP address.
- From `web_app_1`, test communication with `web_app_3` using its IP address.
- Observe and compare the communication behaviour of containers connected to different networks.

#### Exercise 3: Exploring Host Networking
- Create a fourth container named `web_app_4` using the host network mode.
- Inspect the container's network configuration.
- Examine the IP address information provided by Docker and investigate how host networking works in the current environment.

#### Bonus: Container Management
- Explore commands for displaying container IDs.
- Practise stopping all running containers.
- Practise removing containers, including stopped containers.



### Activity 2 — Networking with Ubuntu

Use the official Ubuntu image to explore communication between containers connected to a custom Docker bridge network.

#### Exercise 1: Creating a Bridge Network
- Create a custom Docker network using the bridge driver.

#### Exercise 2: Creating Ubuntu Containers
- Create two Ubuntu containers and connect both to the network created for this activity.

#### Exercise 3: Preparing the Containers
- Install the `ping` utility in the Ubuntu containers when necessary.
- Identify the IP addresses of both containers.

#### Exercise 4: Testing Container Connectivity
- Test communication between the two containers using their IP addresses.
- Test communication between the two containers using their names.
- Observe the results and compare the two methods of communication.

## Learning Objectives

By completing these activities, learners will explore Docker's default bridge network, custom bridge networks and host networking, practise inspecting container network configurations, and investigate communication between containers by IP address and name.
