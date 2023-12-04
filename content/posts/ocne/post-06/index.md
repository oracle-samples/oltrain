---
title: "Deploy Oracle Cloud Native Environment"
date: 2022-05-18
draft: false
summary: "Oracle Cloud Native Environment is a fully integrated suite for the development and management of cloud native applications.  The Kubernetes module is the core module. It is used to deploy and manage containers and also automatically installs and configures CRI-O, runC and Kata Containers.  CRI-O manages the container runtime for a Kubernetes cluster.  The runtime may be either runC or Kata Containers."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Deploy Oracle Cloud Native Environment](https://luna.oracle.com/lab/d18fe294-efb5-4498-9e7b-d5cc724d8619)

:spiral_notepad: [Deploy Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-install)

## Details

Oracle Cloud Native Environment is a fully integrated suite for the development and management of cloud native applications.  The Kubernetes module is the core module. It is used to deploy and manage containers and also automatically installs and configures CRI-O, runC and Kata Containers.  CRI-O manages the container runtime for a Kubernetes cluster.  The runtime may be either runC or Kata Containers.

### Objectives

In this tutorial, you will learn how to:

- Install Oracle Cloud Native Environment on a 3-node cluster
- Configure x.509 Private CA Certificates
- Configure Oracle Cloud Native Environment on a 3-node cluster
- Verify the install completed successfully

### Prerequisites

The tutorial uses the following system:

- 3 Oracle Linux systems to use as:
  - Operator node (ocne-operator)
  - Kubernetes control plane node (ocne-control-01)
  - Kubernetes worker node (ocne-worker-01)

- Each system should have a minimum of the following installed:
  - Latest Oracle Linux (x86_64) installed and running the Unbreakable Enterprise Kernel Release 7 (UEK R7)

- This environment is pre-configured with the following:
  - An Oracle user account with 'sudo' access
  - Key-based SSH, also known as passwordless SSH, between the instances
