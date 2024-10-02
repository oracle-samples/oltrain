---
title: "Use Taints and Tolerations"
date: 2024-10-02
draft: false
summary: "Learn to use taints and tolerations with Oracle Cloud Native Environment."
tags: ["ocne", "ocne2", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/19319fb4-f993-4f5b-b1da-33b73c6a4f39)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-taints)

## Details

The ability to influence the way Pods are [scheduled](https://kubernetes.io/docs/concepts/scheduling-eviction/) to provide the best performance, reduce running costs, and make Kubernetes cluster management easier is an essential skill for an administrator to master. Taints and tolerations work with [Node Affinity](https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/#affinity-and-anti-affinity) to attract Pods to a set of nodes. [Taints and tolerations](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/) have the opposite effect by allowing nodes to repel Pods. Frequent use cases for taints and tolerations include:

- Identifying nodes with special hardware.
- The ability to dedicate nodes to specific application Pods.
- The ability to define custom conditions to evict a Pod from a node.

*Taints* allow the Kubernetes administrator to prevent unwanted Pods from executing on a predefined set of nodes. *Tolerations* allow any Pods to deploy onto a node with a matching taint. Together, these allow the administrator to fine-tune how Pods schedule to nodes.

**Important:** Taints and tolerations **cannot ensure that a Pod schedules to a specific node**. The Kubernetes scheduler can deploy a Pod onto any node without a taint that repels it. Instead, use node affinity when controlling where Pod scheduling is required.

### Objectives

In this tutorial, you will learn:

- The difference between a taint and a toleration
- How to use taints and tolerations to influence application deployment on Oracle Cloud Native Environment

### Prerequisites

- Installation of Oracle Cloud Native Environment
  - a single control node and two worker nodes
