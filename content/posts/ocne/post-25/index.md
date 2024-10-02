---
title: "Use Labels and Node Selectors"
date: 2024-10-2
draft: false
summary: "Learn to use labels and node selectors with Oracle Cloud Native Environment."
tags: ["ocne", "ocne2", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/81c57622-f1dc-4a06-a714-96aae8729b38)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-labels)

## Details

The ability to influence how Kubernetes [schedules](https://kubernetes.io/docs/concepts/scheduling-eviction/) Pods to provide the best performance, reduce running costs, and more easily simplify cluster management is a vital skill for an administrator to master. Many Kubernetes clusters have nodes with varying capabilities, for example:

- GPU card (for machine learning applications)
- SSD disk (for applications requiring fast data access)
- High-end CPU (for CPU-intensive tasks)

Administrators use several ways to influence how the Kubernetes scheduler deploys applications to specific nodes. This tutorial covers using labels and node selectors, which are the simplest way to assign Pods to nodes.

### Objectives

In this tutorial, you will learn:

- How to review and set labels on nodes
- How to define and use a node selector to influence an application deployment

### Prerequisites

- Installation of Oracle Cloud Native Environment
  - a single control node and two worker nodes
