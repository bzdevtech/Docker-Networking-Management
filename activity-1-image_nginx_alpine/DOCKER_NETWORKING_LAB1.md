
# Activity 1 — Networking with an Existing Docker Image

## Objective

Explore Docker networking and understand how containers communicate using different network configurations.

## Docker Image

Reuse the Nginx-based static website image created during **Lab 2 — Docker Image Management**.

You can obtain the image using either of the following options.

### Option 1 — Use the Prebuilt Image from Docker Hub

- Docker Hub repository: https://hub.docker.com/r/tsebaze/static_site_image
- Image tag: `labs2-v1`
- Full image reference: `tsebaze/static_site_image:labs2-v1`

### Option 2 — Build the Image from GitHub Source Code

- GitHub repository: https://github.com/bzdevtech/Docker-Image-Management

Use the source code and Dockerfile to build the image locally.

## Exercise 1 — Default Bridge Network

- Create two containers named `web_app_1` and `web_app_2` using the existing Docker image.
- Do not explicitly specify a network or publish any ports.
- Inspect both containers and identify their network configuration and IP addresses.
- Enter `web_app_1` and test communication with `web_app_2` using its IP address.
- Record your observations.

## Exercise 2 — Custom Bridge Network

- Create a custom Docker bridge network named `network-app-3`.
- Create a third container named `web_app_3` and connect it to this network.
- Inspect `web_app_3` to identify its network configuration and IP address.
- From `web_app_1`, test communication with `web_app_3` using its IP address.
- Observe and compare the communication behaviour of containers connected to different networks.

## Exercise 3 — Host Networking

- Create a fourth container named `web_app_4` using host networking.
- Inspect its network configuration.
- Examine the IP address information and investigate how host networking behaves in the current environment.

## Bonus — Container Management

- Explore commands for displaying container IDs.
- Practise stopping all running containers.
- Practise removing containers, including stopped containers.

## Expected Learning Outcomes

By completing this activity, learners should be able to:

- Identify the default bridge network and a custom bridge network.
- Inspect containers and examine their network configuration and IP addresses.
- Test communication between containers.
- Explore host networking.
- Use essential Docker commands to manage containers.
