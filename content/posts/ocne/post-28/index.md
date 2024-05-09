---
title: "Use Stateless Deployments"
date: 2024-05-09
draft: false
summary: "Learn how to use Stateless Deployments with Oracle Cloud Native Environment."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/ec9d9a9c-ad0f-49e2-8304-512046255635)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-deployments)

## Details

There are two primary approaches to managing applications on Kubernetes - StatefulSets and Deployments. StatefulSets, which require persistent storage, manage stateful workloads such as a MySQL deployment on Kubernetes. Deployments provide a way to manage stateless applications such as websites, which often do not need to maintain their internal state.

> **Note:** A [DaemonSets](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/) is a third available Kubernetes controller. Daemonsets ensure a replica of Pod will always run on all or some other cluster's Nodes and are typically used for logging agents, monitoring systems, etc.

### Objectives

In this tutorial, you will learn:

- How to deploy and manage stateless applications
- How to perform a rolling update and rollback

### Prerequisites

- Minimum of a 3-node Oracle Cloud Native Environment cluster:

   - Operator node
   - Kubernetes control plane node
   - Kubernetes worker node

- Each system should have Oracle Linux installed and configured with:

   - An Oracle user account (used during the installation) with sudo access
   - Key-based SSH, also known as password-less SSH, between the hosts
   - Installation of Oracle Cloud Native Environment
