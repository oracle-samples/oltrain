---
title: "Deploy an External Load Balancer"
date: 2022-07-29
draft: false
summary: "Learn how to deploy an external load-balancer with Oracle Cloud Native Environment."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/be8d99fc-44c3-4062-a3c3-95e982243ccf)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-install-ha-oci)

## Details

Oracle Cloud Native Environment is a fully integrated suite for developing and managing cloud native applications. The Kubernetes module is the core module. It deploys and manages containers and automatically installs and configures CRI-O and RunC. CRI-O manages the container runtime for a Kubernetes cluster, which defaults to RunC.

### Objectives

At the end of this tutorial, you should be able to do the following:

- Configure the Kubernetes cluster with the Oracle Cloud Infrastructure load balancer to enable high availability
- Configure Oracle Cloud Native Environment on a 5-node cluster
- Verify Load Balancer failover between the control plane nodes completes successfully

> **Support Note:** We recommend using an external load balancer such as Oracle Cloud Infrastructure Load Balancer for production deployments.

### Prerequisites

The tutorial uses the following host systems:

- 6 Oracle Linux instances for Oracle Cloud Native Environment:
  - Operator node (_ocne-operator_)
  - 3 Kubernetes control plane nodes (_ocne-control-01, ocne-control-02, ocne-control-03_)
  - 2 Kubernetes worker nodes (_ocne-worker-01, ocne-worker-02_)

- An Oracle Linux system for installing kubectl (devops-node)

  > **Note:**  We recommend that production environments have a cluster with at least five control plane nodes and three worker nodes.

- Configure each system with the following:
  - The latest Oracle Linux with the Unbreakable Enterprise Kernel Release 7 (UEK R7)
  - An `oracle` user account with `sudo` access
  - Key-based SSH, also known as passwordless SSH, between the instances
