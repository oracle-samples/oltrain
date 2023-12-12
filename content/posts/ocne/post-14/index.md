---
title: "Scale a Kubernetes Cluster"
date: 2022-09-06
draft: false
summary: "This tutorial demonstrates how to scale an existing Kubernetes cluster in Oracle Cloud Native Environment.
Scaling up a Kubernetes cluster means adding nodes; likewise, scaling down occurs by removing nodes. Nodes can be either control plane or worker nodes. Oracle recommends against scaling the cluster up and down at the same time. Instead, perform a scale up and then down in two separate commands."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6c9e4d88-27e7-43bd-9366-0693fb8e4d3a)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-scale/)

## Details

This tutorial demonstrates how to scale an existing Kubernetes cluster in Oracle Cloud Native Environment.

Scaling up a Kubernetes cluster means adding nodes; likewise, scaling down occurs by removing nodes. Nodes can be either control plane or worker nodes. Oracle recommends against scaling the cluster up and down at the same time. Instead, perform a scale up and then down in two separate commands.

We recommend scaling the Kubernetes cluster control plane or worker nodes in odd numbers to avoid split-brain scenarios and maintain the quorum. For example, 3, 5, or 7 control plane or worker nodes ensure the reliability of the cluster.

We start with an existing Highly Available Kubernetes cluster running on Oracle Cloud Native Environment that consists of the following:

The starting deployment consists of the following:

- 1 Operator Node
- 3 Control Plane Nodes
- 5 Worker Nodes

It builds upon the labs:

- [Deploy Oracle Cloud Native Environment](https://luna.oracle.com/lab/d18fe294-efb5-4498-9e7b-d5cc724d8619/steps)
- [Deploy an External Load Balancer with Oracle Cloud Native Environment](https://luna.oracle.com/lab/be8d99fc-44c3-4062-a3c3-95e982243ccf/steps)
- [Use OCI Cloud Controller Manager on Oracle Cloud Native Environment](https://luna.oracle.com/lab/5571f277-3eb9-435f-b3b3-fe421fb9747e/steps)

### Objectives

At the end of this tutorial, you should be able to do the following:

- Add two new control plane nodes and two new worker nodes to a cluster
- Scale down the cluster by removing the same nodes from the cluster

### Prerequisites

> **Note:** If using the free lab environment these prerequisites are provided as the starting point.

- A Highly Available Kubernetes cluster running on Oracle Cloud Native Environment

- 4 additional Oracle Linux instances to use as:
  - 2 Kubernetes control plane nodes
  - 2 Kubernetes worker nodes

- Access to a Load Balancer such as OCI Load Balancer

- The additional Oracle Linux instances need the following:
  - The same OS and patch level as the original cluster
  - The completion of the [prerequisite steps to install Oracle Cloud Native Environment](https://docs.oracle.com/en/operating-systems/olcne/1.7/start/prereq.html#prereq)
  - Set up the [Kubernetes Nodes](https://docs.oracle.com/en/operating-systems/olcne/1.7/start/install.html#install-node)
