---
title: "Use Labels and Node Selectors"
date: 2024-03-26
draft: false
summary: "This tutorial shows how to use Labels and Node Selectors with Oracle Cloud Native Environment."
tags: ["ocne", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/81c57622-f1dc-4a06-a714-96aae8729b38)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-labels)

## Details

The ability to influence how Kubernetes schedules Pods to provide the best performance, reduce running costs and more easily simplify cluster management is a vital skill for an administrator to master. Many Kubernetes clusters have nodes with varying capabilities, for example:

- GPU card (for machine learning applications)
- SSD disk (for applications requiring fast data access)
- High-end CPU (for CPU-intensive tasks)

Administrators use several ways to influence how the Kubernetes scheduler deploys applications to specific nodes. This tutorial covers using labels and nodeSelector (the simplest way to assign pods to nodes).

### Objectives

You will learn:

- How to review and set labels on Nodes.
- How to define and use a nodeSelector to influence an application deployment.

### Prerequisites

- 4 Oracle Linux systems to use as:
  - Operator node (ocne-operator-01)
  - Kubernetes control plane node (ocne-control-01)
  - Kubernetes worker nodes (ocne-worker-01 & ocne-worker-02)

- Each system should have the latest Oracle Linux 8 (x86_64) installed

- This environment is pre-configured with:
  - An Oracle user account (used during the installation) with sudo access
  - Key-based SSH, also known as password-less SSH, between the hosts
  - Installation of Oracle Cloud Native Environment
