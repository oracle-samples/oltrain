---
title: "Scale an Oracle Cloud Native Environment Cluster"
date: 2024-12-18
draft: false
summary: "Learn how to configure cluster scaling on Oracle Cloud Native Environment."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/9d258745-5ca3-4e5a-9467-66be43d12a8a)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-scale)

## Details

Scaling up a Kubernetes cluster means adding nodes; likewise, scaling down occurs by removing nodes. These nodes can be either control plane or worker nodes. Oracle recommends against scaling the cluster up and down simultaneously but instead performing a scale up and down in two separate commands.

Scaling the Kubernetes cluster control plane or worker nodes in odd numbers is recommended to avoid split-brain scenarios and maintain the quorum. For example, 3, 5, or 7 control plane nodes or worker nodes ensure the cluster's reliability.

### Objectives

In this tutorial, you'll learn how to use `kubectl scale` and `kubectl edit` to:

- Add a new control plane and worker nodes to a Kubernetes cluster
- Remove control plane nodes and worker nodes from a Kubernetes cluster

### Prerequisites

- Minimum of one Oracle Linux instance
  - Runs `ocne` and `libvirt` ephemeral cluster

- OCI cluster creation requires access to the following resources in an Oracle Cloud Infrastructure tenancy:

  - Virtual cloud network with four subnets
  - Network load balancer
  - Object Storage bucket with minimum 5 GiB available
  - Compute Custom Image
  - Compute Arm Shape for the control plane node
    - VM.Standard.A1.Flex with two OCPU and 12 memory
  - Compute for each additional control plane and worker node
    - VM.Standard.E4.Flex with four OCPU and 64 memory
