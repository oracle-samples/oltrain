---
title: "Deploy and use Ingress-Nginx Controller on Oracle Cloud Native Environment"
date: 2024-06-12
draft: false
summary: "Learn how to deploy and use Ingress-Nginx Controller on Oracle Cloud Native Environment"
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/18559783-6392-45f0-ac90-622eff1a6ce9)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-ingress-nginx)

## Details

[Ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/) is a Kubernetes API object that manages external access to a cluster's services. The [Ingress-Nginx Controller](https://kubernetes.github.io/ingress-nginx/) uses [NGINX](https://nginx.org/) as a reverse proxy and load balancer that can load-balance Websocket, gRPC, TCP, and UDP applications.

### Objectives

In this tutorial, you will learn:

   - How to install and access the Ingress-Nginx Controller

### Prerequisites

- Minimum of a 3-node Oracle Cloud Native Environment cluster:

   - Operator node
   - Kubernetes control plane node
   - Kubernetes worker node

- Each system should have Oracle Linux installed and configured with:

   - An Oracle user account (used during the installation) with sudo access
   - Key-based SSH, also known as password-less SSH, between the hosts
   - Installation of Oracle Cloud Native Environment with the OCI Cloud Controller Manager
