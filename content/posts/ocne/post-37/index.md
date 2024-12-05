---
title: "Run Ingress-nginx with MetalLB"
date: 2024-10-08
draft: false
summary: "Learn to deploy and use the Ingress-Nginx Controller with MetalLB on Oracle Cloud Native Environment."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/5b1cf1fd-fb87-4e7b-aa67-f19f5114d104)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-metallb-ingress-nginx)

## Details

[Network load balancers](https://kubernetes.io/docs/concepts/services-networking/) such as [MetalLB](https://metallb.universe.tf/) provide a method of externally exposing Kubernetes applications. A Kubernetes [LoadBalancer](https://kubernetes.io/docs/concepts/services-networking/service/#loadbalancer) service creates a network load balancer that provides and exposes an external IP address for connecting to an application from outside the cluster.

With the external IP address exposed, administrators of a Kubernetes cluster can then manage access to applications via an [Ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/). An Ingress is a Kubernetes API object that manages external access to a cluster's services. The [Ingress-Nginx Controller](https://kubernetes.github.io/ingress-nginx/) uses [NGINX](https://nginx.org/) as a reverse proxy and load balancer that can load-balance Websocket, gRPC, TCP, and UDP applications.

### Objectives

In this tutorial, you will learn:

- How to install and configure MetalLB
- How to install and access the Ingress-Nginx Controller

### Prerequisites

- Installation of Oracle Cloud Native Environment
  - a single control node and four worker nodes
