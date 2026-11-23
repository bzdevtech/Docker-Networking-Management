
# Activity 2 — Networking with Ubuntu

## Objective

Explore communication between two Ubuntu containers connected to a custom Docker bridge network.

## Exercise 1 — Create a Bridge Network

- Create a custom Docker network using the bridge driver.
- Verify that the network has been created successfully.

## Exercise 2 — Create Two Ubuntu Containers

- Use the official Ubuntu Docker image.
- Create two Ubuntu containers and connect both to the network created for this activity.
- Ensure that both containers remain running for the networking exercises.

## Exercise 3 — Prepare the Containers

- Install the `ping` utility in the Ubuntu containers when necessary.
- Identify the IP addresses of both containers.

## Exercise 4 — Test Container Connectivity

- Test communication between the two containers using their IP addresses.
- Test communication between the two containers using their names.
- Observe the results and compare the two methods of communication.

## Expected Learning Outcomes

By completing this activity, learners should be able to:

- Create and inspect a custom Docker bridge network.
- Run Ubuntu containers on the same network.
- Install and use network diagnostic tools.
- Test communication between containers using IP addresses and names.
- Interpret connectivity test results.