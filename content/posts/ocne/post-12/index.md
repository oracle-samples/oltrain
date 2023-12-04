---
title: "Use MetalLB with Oracle Cloud Native Environment"
date: 2022-08-15
draft: false
summary: "[MetalLB](https://metallb.universe.tf/) is a network load balancer for Kubernetes applications deployed with Oracle Cloud Native Environment that runs on bare metal hosts. MetalLB allows you to use Kubernetes LoadBalancer services, which traditionally use a cloud provider's network load balancer, in bare metal environments."
tags: ["ocne", "lab", "tutorial"]
showDate: true
---

## Links

:crescent_moon: [Use MetalLB with Oracle Cloud Native Environment](https://luna.oracle.com/lab/d931637d-4e6b-4a46-ba17-810a942c4309)

:spiral_notepad: [Use MetalLB with Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-metallb)

## Details

[Network load balancers](https://kubernetes.io/docs/concepts/services-networking/) provide a method of externally exposing Kubernetes applications. A Kubernetes [LoadBalancer](https://kubernetes.io/docs/concepts/services-networking/service/#loadbalancer) service creates a network load balancer that provides and exposes an external IP address for connecting to an application from outside the cluster.

[MetalLB](https://metallb.universe.tf/) is a network load balancer for Kubernetes applications deployed with Oracle Cloud Native Environment that runs on bare metal hosts. MetalLB allows you to use Kubernetes LoadBalancer services, which traditionally use a cloud provider's network load balancer, in bare metal environments.

### Objectives

At the end of this tutorial, you should be able to set up and use the MetalLB module for Kubernetes applications using MetalLB and Oracle Cloud Native Environment.

### Prerequisites

The tutorial uses the following host systems:

- 6 Oracle Linux instances for Oracle Cloud Native Environment:
  - Operator node (_ocne-operator_)
  - 3 Kubernetes control plane nodes (_ocne-control-01, ocne-control-02, ocne-control-03_)
  - 2 Kubernetes worker nodes (_ocne-worker-01, ocne-worker-02_)


  > **Note:**  We recommend that production environments have a cluster with at least five control plane nodes and three worker nodes.

- A virtual IP address for the primary control plane node. Do not use this IP address on any of the nodes. The load balancer dynamically sets the IP address to the control plane node assigned as the primary controller.

> **Oracle Support Disclaimer:** If you are deploying to Oracle Cloud Infrastructure, your tenancy requires enabling a new feature introduced in OCI: Layer 2 Networking for VLANs within your virtual cloud networks (VCNs). The OCI Layer 2 Networking feature is not generally available, although the free lab environment's tenancy enables this feature. If you have a use case, please work with your technical team to get your tenancy listed to use this feature.

- Configure each system with the following:
  - The latest Oracle Linux with the Unbreakable Enterprise Kernel Release 7 (UEK R7)
  - An `oracle` user account with `sudo` access
  - Key-based SSH, also known as passwordless SSH, between the instances
  - Install Oracle Cloud Native Environment ready for creating the environment and installing modules
  - Create a VLAN and assign IPv4 addresses
