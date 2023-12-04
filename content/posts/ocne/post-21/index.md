---
title: "Run KubeVirt"
date: 2023-09-18
draft: false
summary: "KubeVirt is a virtualization technology to create and manage virtual machines in Kubernetes. Administrators create these virtual machines using the kubectl command and Kubernetes custom resource definitions (CRDs)."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/87d85c56-d929-45bc-aa8c-3f51cd584b2d)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-kubevirt/)

## Details

KubeVirt is a virtualization technology to create and manage virtual machines in Kubernetes. Administrators create these virtual machines using the kubectl command and Kubernetes custom resource definitions (CRDs). As with any container image within Kubernetes, it requires persistent storage to maintain its state. Hence, our need for Rook and Ceph.

Rook is a cloud-native storage orchestrator platform that enables Ceph storage for our Kubernetes cluster. Rook deploys as a Kubernetes operator inside a Kubernetes cluster and automates the tasks to provision and de-provision Ceph-backed persistent storage using the Kubernetes Container Storage Interface (CSI).

While Ceph allows the creation of block and object storage, there also exists a shared file system storage. This type uses a CephFilesystem (CephFS) to mount a shared POSIX (Portable Operating System Interface) compliant folder into one or more pods. This storage type is similar to NFS (Network File System) shared storage or CIFS (Common Internet File System) shared folders.

This tutorial guides users on deploying KubeVirt with Ceph storage managed by Rook on Oracle Cloud Native Environment.

### Objectives

At the end of this tutorial, you should be able to do the following:

- Install the Rook operator
- Configure Ceph storage
- Install KubeVirt
- Create and Deploy a VM

### Prerequisites

- Running Oracle Cloud Native Environment cluster consisting of an operator node, two control plane nodes, and three worker nodes.
- Each worker node contains an attached unformatted block volume
- An available container registry to store container image VMs.
