---
title: "Deploy HAProxy"
date: 2023-03-09
draft: false
summary: "Learn to run and configure HAProxy in a container using Podman."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/a9eb9ff9-b56d-4ddc-9283-b72467d78128)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-podman-haproxy/)

## Details

HAProxy is a well-known and widely used open-source solution that delivers load balancing and proxy services for HTTP (Layer 7) and TCP (Layer 4), achieved by spreading incoming requests across multiple servers. The load balancer can also detect if any servers in its pool become unresponsive and automatically stop forwarding incoming traffic to them. For more details on the services HAProxy *does* and *does not* provide, please refer to the [upstream documentation](https://docs.haproxy.org). You can install HAProxy locally using packages provided by Oracle or run as a container. This tutorial covers the latter using Podman.

### Objectives

In this tutorial, you'll learn how to:

  - Use HAProxy as a Podman-based container 
  - Configure a simple deployment using three backend servers
  - Confirm the deployment runs as expected

 > **Note:** The steps do not include configuring HAProxy to use certificates, which we recommend for production environments.

### Prerequisites

- Minimum of 4 Oracle Linux systems

   - HAProxy node
   - 3 Web Application nodes

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Key-based SSH, also known as password-less SSH, between the hosts
    - Podman and cURL packages
    - Access to the Internet

