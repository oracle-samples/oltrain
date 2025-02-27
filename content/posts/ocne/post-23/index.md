---
title: "Use Persistent Volumes and Persistent Volume Claims"
date: 2025-02-27
draft: false
summary: "This tutorial shows how to create and use Persistent Volumes and Persistent Volume Claims with Oracle Cloud Native Environment."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/cdf43182-16c7-4c42-9a91-6052a5934184)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-pv/#introduction)

## Details

Because container-based applications are stateless by default, any file updates during the container lifetime are lost. However, if your application is stateful, the ability to persist any changes to the filesystem becomes relevant. It is this requirement that has led to Kubernetes supporting many types of volumes. Many volume types that you may have encountered already are [ephemeral](https://kubernetes.io/docs/concepts/storage/ephemeral-volumes/) (they only exist during the pod lifetime). Kubernetes also supports [persistent](https://kubernetes.io/docs/concepts/storage/persistent-volumes/) volumes, which persist any data stored beyond the pod lifetime. There are several [Persistent Volume types](https://kubernetes.io/docs/concepts/storage/persistent-volumes/#types-of-persistent-volumes) supported by Kubernetes, and this tutorial will demonstrate one of the simplest - the `local` type, which stores data on devices stored locally on one of the cluster nodes.

This tutorial shows how to create and use Persistent Volumes and Persistent Volume Claims with Oracle Cloud Native Environment (Oracle CNE). Persistent Volumes and Persistent Volume Claims work together to provide persistence to any container-based applications deployed onto Oracle CNE. You will start by covering how to use Persistent Volumes initially, then cover the use of Persistent Volume Claims.

### Objectives

In this tutorial, you will learn to:

- Install the prerequisites for the *oci* provider
- Use the *oci* provider to create and manage a Kubernetes cluster
- The difference between a Persistent Volume (PV) and a Persistent Volume Claim (PVC)
- How to use Persistent Volumes and Persistent Volume Claims

### Prerequisites

- Minimum of one Oracle Linux instance

- Each system should have Oracle Linux installed and configured with:

  - An Oracle user account (used during the installation) with sudo access
  - Key-based SSH, also known as password-less SSH, between the hosts

- OCI cluster creation requires access to the following resources in an Oracle Cloud Infrastructure tenancy:

  - Virtual cloud network with four subnets
  - Network load balancer
  - Object Storage bucket with minimum 5 GiB available
  - Compute Custom Image
  - Compute Arm Shape for the control plane node
    - VM.Standard.A1.Flex with two OCPU and 12 memory
  - Compute for each additional control plane and worker node
    - VM.Standard.E4.Flex with four OCPU and 64 memory 
