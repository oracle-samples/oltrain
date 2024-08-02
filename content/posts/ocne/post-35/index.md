---
title: "Install kind"
date: 2023-08-07
draft: false
summary: "Learn to install a local Kubernetes cluster using kind on Oracle Linux to develop for Cloud Native environments."
tags: ["ocne", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/30610e81-95e7-4c54-85bc-efcb5e757e04)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-kind)

## Details

[*kind*](https://kind.sigs.k8s.io/) is an open-source tool for running a locally hosted Kubernetes cluster using Podman containers as the cluster nodes. It provides a way for both developers and DevOps administrators to quickly create a Kubernetes cluster on a single machine without requiring the usual complicated and lengthy setup that would entail.

### Objectives

In this tutorial, you'll learn how to:

- Install `kubectl`
- Install *kind*
- Use *kind* to start a single-node Kubernetes cluster

### Prerequisites

- Minimum of a single Oracle Linux 9 or later system

- Each system should have Oracle Linux installed and configured with:
    - A non-root user account with sudo access
    - Podman and cURL packages
    - Cgroups v2
