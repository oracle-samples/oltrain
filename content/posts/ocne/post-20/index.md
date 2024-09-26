---
title: "Use Kubectl to Manage Kubernetes Clusters and Nodes"
date: 2024-09-26
draft: false
summary: "Learn how to use kubectl to manage Kubernetes Clusters and Nodes with Oracle Cloud Native Environment."
tags: ["ocne", "ocne2", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/4b16d141-4825-4d54-98f3-ce7babbea45c)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-kubectl-cluster/)

## Details

Although graphical tools can manage Kubernetes, many administrators prefer to use command-line tools. The command line tool provided within the Kubernetes ecosystem is called [kubectl](https://kubernetes.io/docs/reference/kubectl/kubectl/). Kubectl is a versatile tool used to deploy and inspect the configurations and logs of the cluster resources and applications. Kubectl achieves this by using the Kubernetes API to authenticate with the control Node of the Kubernetes cluster to complete any management actions requested by the administrator. 

Most of the operations/commands available for kubectl provide administrators with the ability to deploy and manage applications deployed onto the Kubernetes cluster and inspect and manage the Kubernetes cluster resources.

> **Note:** Many kubectl commands have the `--all-namespaces` option appended. For this reason, a shorthand for this option is the `-A` flag. This tutorial often uses `kubectl -A` instead of `kubectl --all-namespaces`.

### Objectives

This tutorial builds on the basic commands introduced in [Introducing Kubectl with Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-kubectl-intro). If this is your first encounter using *kubectl*, you may find it beneficial to start there. This tutorial introduces how *kubectl* can manage individual Kubernetes Nodes and any application(s) deployed onto them. The specific areas of Node management introduced in this tutorial are:

   - Querying Cluster Information
   - Querying Node information
   - Deploying an example application (Nginx)
   - Introducing new concepts such as:
      - Cordoning/Uncordoning and Draining Nodes
      - Taints and Tolerations

This tutorial only uses `kubectl` to view the current configuration information.

### Prerequisites

- Installation of Oracle Cloud Native Environment
   - a single control node and 3 worker nodes
