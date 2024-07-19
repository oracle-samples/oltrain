---
title: "Use Kubectl to Manage Kubernetes Clusters and Nodes"
date: 2023-05-31
draft: false
summary: "Learn how to use kubectl to manage Kubernetes Clusters and Nodes with Oracle Cloud Native Environment."
tags: ["ocne", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/4b16d141-4825-4d54-98f3-ce7babbea45c)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-kubectl-cluster/)

## Details

Although graphical tools can manage Kubernetes, many administrators prefer to use command-line tools. The command line tool provided within the Kubernetes ecosystem is called [kubectl](https://kubernetes.io/docs/reference/kubectl/kubectl/). Kubectl is a versatile tool used to deploy and inspect the configurations and logs of the cluster resources and applications. Kubectl achieves this by using the Kubernetes API to authenticate with the Control Node of the Kubernetes cluster to complete any management actions requested by the administrator.
Most of the operations/commands available for kubectl provide administrators with the ability to deploy and manage applications deployed onto the Kubernetes cluster and inspect and manage the Kubernetes cluster resources.

> **Note:** Many kubectl commands have the `--all-namespaces` option appended. For this reason, a shorthand for this option is the `-A` flag. This lab uses kubectl `-A` instead of `kubectl --all-namespaces` in preference.

### Objectives

This tutorial builds on the basic commands introduced in a previous tutorial, [Introducing Kubectl with Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-kubectl-intro). If this is your first encounter using kubectl, you may find it beneficial to start there. This tutorial introduces how kubectl can manage individual Kubernetes Nodes and any application(s) deployed onto them. The specific areas of Node management introduced in this tutorial are:

- Querying Cluster Information
- Querying Node information
- Deploying an example application (Nginx)
- Introducing new concepts such as:
  - Cordoning/Uncordoning and Draining Nodes
  - Taints and Tolerations

This tutorial only uses kubectl to view the current configuration information.

### Prerequisites

- 5 Oracle Linux systems to use:
  - 1-off Operator node (ocne-operator)
  - 1-off Kubernetes control plane node (ocne-control)
  - 3-off Kubernetes worker node (ocne-worker)

Each system should have the latest Oracle Linux 8 (x86_64)

- The environment is pre-configured with the following;
  - An oracle user account (used during the installation) with sudo access
  - Key-based SSH, also known as passwordless SSH, between the hosts
  - Installation of Oracle Cloud Native Environment and CCM module
