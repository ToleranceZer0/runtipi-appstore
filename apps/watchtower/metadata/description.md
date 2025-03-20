# Watchtower

Watchtower

A process for automating Docker container base image updates.

Circle CI codecov GoDoc Go Report Card latest version Apache-2.0 License Codacy Badge All Contributors Pulls from DockerHub
Quick Start

With watchtower you can update the running version of your containerized app simply by pushing a new image to the Docker Hub or your own image registry.

Watchtower will pull down your new image, gracefully shut down your existing container and restart it with the same options that were used when it was deployed initially. Run the watchtower container with the following command:

$ docker run --detach \
    --name watchtower \
    --volume /var/run/docker.sock:/var/run/docker.sock \
    containrrr/watchtower

Watchtower is intended to be used in homelabs, media centers, local dev environments, and similar. We do not recommend using Watchtower in a commercial or production environment. If that is you, you should be looking into using Kubernetes. If that feels like too big a step for you, please look into solutions like MicroK8s and k3s that take away a lot of the toil of running a Kubernetes cluster.
Documentation
The full documentation is available at https://containrrr.dev/watchtower.

