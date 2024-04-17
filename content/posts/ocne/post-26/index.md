---
title: "Use Affinity"
date: 2024-04-16
draft: false
summary: "This tutorial shows how to use Affinity and Anti-affinity with Oracle Cloud Native Environment."
tags: ["ocne", "lab", "tutorial", "ocne-k8s", "affinity"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/91b487c8-7c50-4daa-b38c-9e11f6f11175)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-affinity)

## Details

The ability to influence how Kubernetes schedules Pods to provide the best performance, reduce running costs and simplify cluster management is an important skill for an administrator to master.

But what happens if you have several applications deployed to your Kubernetes cluster that would run more efficiently on some nodes rather than others? Administrators use several ways to influence how the Kubernetes scheduler assigns application pods to specific nodes within your cluster. Node Affinity and Pod Affinity/Anti-affinity help by providing flexible rules that govern how the Kubernetes scheduler deploys pods to nodes in the cluster. This tutorial covers using Affinity and Anti-Affinity.

### Objectives

You will learn:

- How to use Affinity.
- How to use Anti-Affinity.

### Prerequisites

- 6 Oracle Linux systems to use as:
  - Operator node (ocne-operator-01)
  - Kubernetes control plane node (ocne-control-01)
  - Kubernetes worker nodes (ocne-worker-01, ocne-worker-02, ocne-worker-03 & ocne-worker-04)

- Each system should have the latest Oracle Linux 8 (x86_64) installed and configured with:

  - An Oracle user account (used during the installation) with sudo access
  - Key-based SSH, also known as password-less SSH, between the hosts
  - Installation of Oracle Cloud Native Environment
