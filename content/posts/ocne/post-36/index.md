---
title: "Install libvirt Cluster"
date: 2024-09-25
draft: false
summary: "Learn to create a Kubernetes Cluster using the *libvirt* provider with the Oracle Cloud Native Environment CLI."
tags: ["ocne2", "lab", "tutorial", "ocne2-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6c3fbf57-8bae-4247-9b09-360b1a513871)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-install-libvirt)

## Details

Oracle Cloud Native Environment includes a CLI that can manage the life cycle of Kubernetes clusters using OSTree-based container images. Oracle Cloud Native Environment includes several provider types you can use to create a Kubernetes cluster, and this tutorial introduces how to use the `ocne cluster` command to create Kernel-based Virtual Machines (KVM) using the *libvirt* provider.

The *libvirt* provider is the default Oracle Cloud Native Environment provider and provisions Kubernetes clusters using KVM. Oracle Cloud Native Environment uses the Oracle KVM stack to install *libvirt* because this version offers many more features for Oracle Linux-based systems.

For more information about Oracle Cloud Native Environment 2, please refer to the [Release 2 Documentation](https://docs.oracle.com/en/operating-systems/olcne/) site.

### Objectives

In this tutorial, you'll learn to:

- Install the *libvirt* provider
- Install the Oracle Cloud Native Environment Command Line Interface (CLI)
- Use the *libvirt* provider to create and manage a Kubernetes cluster

### Prerequisites

- Minimum of one Oracle Linux instance

- Each system should have Oracle Linux installed and configured with:

   - An Oracle user account (used during the installation) with sudo access
   - Key-based SSH, also known as password-less SSH, between the hosts