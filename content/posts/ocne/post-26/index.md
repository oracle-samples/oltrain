---
title: "Use Affinity"
date: 2024-10-03
draft: false
summary: "Learn to use affinity and anti-affinity with Oracle Cloud Native Environment."
tags: ["ocne", "ocne2", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/91b487c8-7c50-4daa-b38c-9e11f6f11175)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-affinity)

## Details

The ability to influence how Kubernetes [schedules](https://kubernetes.io/docs/concepts/scheduling-eviction/) Pods to provide the best performance, reduce running costs, and simplify cluster management is an essential skill for an administrator to master.

But what happens if you have several applications deployed to your Kubernetes cluster that would run more efficiently on some nodes rather than others? Administrators use several ways to influence how the Kubernetes scheduler assigns application Pods to specific nodes within your cluster. Node Affinity, Pod affinity, and Pod anti-affinity help by providing flexible rules that govern how the Kubernetes scheduler deploys Pods to nodes in the cluster.

### Objectives

In this tutorial, you will learn:

- How to use affinity
- How to use anti-affinity

### Prerequisites

- Installation of Oracle Cloud Native Environment
  - a single control node and four worker nodes
