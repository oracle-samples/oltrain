---
title: "Install Minikube"
date: 2022-04-19
draft: false
summary: "Minikube is a popular tool for developers and administrators to run a fully functional Kubernetes cluster in their local environment. Although minikube is cross-platform, this tutorial only guides you through the installation and configuration of minikube with the podman driver."
tags: ["k8s", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/8b2f7860-3204-4cd3-8d55-3f6de9ca03c2)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ol-minikube)

## Details

Minikube is a popular tool for developers and administrators to run a fully functional Kubernetes cluster in their local environment.
Although minikube is cross-platform, this tutorial only guides you through the installation and configuration of minikube with the podman driver.

### Objectives

In this tutorial, you will learn how to:

- Download & install minikube and Podman on Oracle Linux
- Configure minikube to use the podman driver
- Verify the installation of minikube

### Prerequisites

The tutorial uses the following system:

- A system with Oracle Linux installed with the following hardware and configuration:
  - 2 CPUs (or more)
  - 2Gb memory (or more)
  - 20Gb free disk space for minikube itself
  - Using minikube requires more space if installing minikube Addons or deploying any projects
  - a non-root user with sudo permissions
