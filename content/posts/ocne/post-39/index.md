---
title: "Use Kubepug"
date: 2024-10-23
draft: false
summary: "Learn to install and run kubepug on Oracle Cloud Native Environment to detect deprecated APIs before upgrading Kubernetes."
tags: ["ocne2", "lab", "tutorial", "ocne2-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/b1ef9efe-adbb-44b1-bd98-8d3b7c5ec0fc)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-kubepug)

## Details

[Kubepug](https://kubepug.xyz/) is an open-source project and program that helps administrators of a Kubernetes cluster upgrade by finding deprecated APIs for resources that require either migration or removal from the cluster.

These different API types are usually deprecated in one version and then removed or deleted in a future version based on a selected lifecycle. Kubepug detects these deprecations or deletions by allowing you to set your Kubernetes version, which it will use to validate your cluster or manifest files.

### Objectives

In this tutorial, you will learn:

- How to install the Kubepug plugin using Krew
- How to run KubePub to determine deprecated clusters and manifests

### Prerequisites

- Installation of Oracle Cloud Native Environment
  - a single control node and one worker node
