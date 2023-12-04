---
title: "Use Gluster"
date: 2022-05-18
draft: false
summary: "Using the Gluster Container Storage Interface module, Oracle Cloud Native Environment administrators can set up statically or dynamically provisioned persistent storage for Kubernetes applications using Gluster Storage."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/5455954d-142c-4801-9f34-5946ad19573d)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-gluster)

## Details

Using the Gluster Container Storage Interface module, Oracle Cloud Native Environment administrators can set up statically or dynamically provisioned persistent storage for Kubernetes applications using Gluster Storage.

The Gluster Container Storage Interface module creates a Kubernetes Glusterfs [StorageClass](https://kubernetes.io/docs/concepts/storage/storage-classes/#glusterfs) provisioner to access existing storage on Gluster. Kubernetes uses the Glusterfs plug-in to provision Gluster volumes for use as Kubernetes [PersistentVolumes](https://kubernetes.io/docs/concepts/storage/persistent-volumes/). The Oracle Cloud Native Environment Platform API Server communicates with the [Heketi](https://github.com/heketi/heketi) API to provision and manage Gluster volumes using PersistentVolumeClaims. When deleting the [PersistentVolumeClaims](https://kubernetes.io/docs/concepts/storage/persistent-volumes/#persistentvolumeclaims), the Gluster volumes automatically get destroyed.

In this example, we will create an integrated system where Kubernetes worker nodes provide persistent storage using [Gluster](https://www.gluster.org/) on Oracle Cloud Native Environment.

### Deprecation Notice for Release 1.6 - Gluster Container Storage Interface Module

The Gluster Container Storage Interface module, used to install Gluster and set up Glusterfs, is deprecated. Future releases may remove the Gluster Container Storage Interface module.

> **Note:** The free lab environment deploys Release 1.6 and may not be updated due to this deprecation notice.

### Objectives

In this tutorial, you will learn how to install and configure Gluster Storage for Oracle Linux on Oracle Cloud Native Environment to create storage volumes for Kubernetes applications.

### Prerequisites

The tutorial uses the following system:

- 5 Oracle Linux systems to use as:
  - Operator node (_ocne-operator)_
  - Kubernetes control plane node (_ocne-control01_)
  - 3 Kubernetes worker nodes (_ocne-worker01, ocne-worker02, ocne-worker03_)

- Systems should have a minimum of the following:
  - Latest Oracle Linux 8 (x86_64) installed and running the Unbreakable Enterprise Kernel Release 6 (UEK R6)

- The pre-configured setup on these systems is:
  - An oracle user account with sudo privileges
  - Passwordless SSH between each node
  - Additional block storage attached to each worker node for Gluster
  - Oracle Cloud Native Environment installed and configured