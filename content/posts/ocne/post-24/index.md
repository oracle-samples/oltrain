---
title: "Use Taints and Tolerations"
date: 2024-03-07
draft: false
summary: "This tutorial shows how to use Taints and Tolerations with Oracle Cloud Native Environment."
tags: ["ocne", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/19319fb4-f993-4f5b-b1da-33b73c6a4f39)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-taints)

## Details

Taints allow the Kubernetes administrator to prevent unwanted Pods from executing on a predefined set of nodes. Tolerations allow any Pods to deploy onto a node with a matching Taint. Together these allow the administrator to fine-tune how Pods schedule to Nodes.

However, it is important to note that taints and tolerations cannot ensure that a pod schedules to a specific node. The Kubernetes scheduler can deploy a pod onto any node without a taint that repels it. Instead, use Node affinity when control over where Pods schedule is required.

This tutorial shows how to create and use Taints and Tolerations with Oracle Cloud Native Environment.

### Objectives

You will learn:

- The difference between a Taint and a Toleration
- How to use Taints and Tolerations to influence application deployment on Oracle Cloud Native Environment.

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
