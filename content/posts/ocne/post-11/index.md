---
title: "Deploy an Internal Load Balancer with Oracle Cloud Native Environment"
date: 2022-07-29
draft: false
summary: "Learn how to deploy an internal load-balancer with Oracle Cloud Native Environment to enable high availability."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Deploy an Internal Load Balancer with Oracle Cloud Native Environment](https://luna.oracle.com/lab/15c6f5a7-9fec-4946-bb42-92dd41310fdf)

:spiral_notepad: [Deploy an Internal Load Balancer with Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-install-ha)

## Details

Oracle Cloud Native Environment is a fully integrated suite for developing and managing cloud native applications. The Kubernetes module is the core module. It deploys and manages containers and automatically installs and configures CRI-O and RunC. CRI-O manages the container runtime for a Kubernetes cluster, which defaults to RunC.

### Objectives

At the end of this tutorial, you should be able to do the following:

- Configure the Kubernetes cluster with an internal load balancer to enable high availability
- Configure Oracle Cloud Native Environment on a 5-node cluster
- Verify keepalived failover between the control plane nodes completes successfully

> **Support Note:** Using the internal load balancer is NOT recommended for production deployments. Instead, please use a correctly configured (external) load balancer.

> **Support Note:** We recommend using an external load balancer such as Oracle Cloud Infrastructure Load Balancer for production deployments.

### Prerequisites

The tutorial uses the following host systems:

- 6 Oracle Linux instances for Oracle Cloud Native Environment:
  - Operator node (_ocne-operator_)
  - 3 Kubernetes control plane nodes (_ocne-control-01, ocne-control-02, ocne-control-03_)
  - 2 Kubernetes worker nodes (_ocne-worker-01, ocne-worker-02_)

- An Oracle Linux system for installing kubectl (devops-node)

  > **Note:**  We recommend that production environments have a cluster with at least five control plane nodes and three worker nodes.

- A virtual IP address for the primary control plane node. Do not use this IP address on any of the nodes. The load balancer dynamically sets the IP address to the control plane node assigned as the primary controller.

> **Oracle Support Disclaimer:** If you are deploying to Oracle Cloud Infrastructure, your tenancy requires enabling a new feature introduced in OCI: Layer 2 Networking for VLANs within your virtual cloud networks (VCNs). The OCI Layer 2 Networking feature is not generally available, although the free lab environment's tenancy enables this feature. If you have a use case, please work with your technical team to get your tenancy listed to use this feature.

- Configure each system with the following:
  - The latest Oracle Linux with the Unbreakable Enterprise Kernel Release 7 (UEK R7)
  - An `oracle` user account with `sudo` access
  - Key-based SSH, also known as passwordless SSH, between the instances
  - Install Oracle Cloud Native Environment ready for creating the environment and installing modules
  - Create a VLAN and assign IPv4 addresses
