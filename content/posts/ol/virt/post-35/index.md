---
title: "Install kind"
date: 2023-08-07
draft: false
summary: "Learn how to install kind using rootless Podman."
tags: ["ol","lab","tutorial","ol-podman"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/30610e81-95e7-4c54-85bc-efcb5e757e04)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/podman-kind)

## Details

[_kind_](https://kind.sigs.k8s.io/) is an open-source tool for running a locally hosted Kubernetes cluster using Podman containers as the cluster nodes. It provides a way for both developers and DevOps administrators to quickly create a Kubernetes cluster on a single machine without requiring the usual complicated and lengthy setup that would entail.

### Objectives

In this lab, you'll learn how to:

- Install Podman
- Install `kubectl`
- Install _kind_
- Start _kind_ using Rootless Podman
- Use _kind_ to start a single-node Kubernetes cluster (control plane and worker on the same node)

### Prerequisites

- A running instance of Oracle Linux 9

