---
title: "Use Stateless Deployments"
date: 2024-09-30
draft: false
summary: "Learn how to use Stateless Deployments with Oracle Cloud Native Environment."
tags: ["ocne", "ocne2", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/ec9d9a9c-ad0f-49e2-8304-512046255635)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-deployments)

## Details

There are two primary approaches to managing applications on Kubernetes - StatefulSets and Deployments. StatefulSets, which require persistent storage, manage stateful workloads such as a MySQL deployment on Kubernetes. Deployments provide a way to manage stateless applications such as websites, which often do not need to maintain their internal state.

A [DaemonSets](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/) is another workload management type available to a Kubernetes controller. Daemonsets ensure a replica of a Pod will always run on all or some of the cluster's Nodes, and you'll typically use it for cluster storage daemons, logging agents, or monitoring systems.

### Objectives

In this tutorial, you will learn:

- How to deploy and manage stateless applications
- How to perform a rolling update and rollback

### Prerequisites

- Installation of Oracle Cloud Native Environment
   - a single control and worker node
