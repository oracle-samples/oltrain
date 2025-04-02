---
title: "Update Kubernetes Version"
date: 2025-04-02
draft: false
summary: "Learn how to upgrade the Kubernetes version in your Oracle Cloud Native Environment cluster."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/14b48272-191c-4c61-9fce-e4200b6af519)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-upgrade-kubernetes)

## Details

Best practices recommend upgrading your Kubernetes cluster as soon after a new release as possible. The reasons to upgrade as quickly as possible include:

- Apply the latest security fixes
- Access stability and performance improvements
- Access new features, APIs & functionality 

This tutorial demonstrates how to upgrade the Kubernetes version used on your Oracle CNE cluster.

For more information about Oracle CNE, please refer to the current [Release Documentation](https://docs.oracle.com/en/operating-systems/olcne/) site.

### Objectives

In this tutorial, you'll learn to:

- Upgrade the Kubernetes version deployed across your cluster

### Prerequisites

- Minimum of one Oracle Linux instance

- Each system should have Oracle Linux installed and configured with:

  - An Oracle user account (used during the installation) with sudo access
  - Key-based SSH, also known as password-less SSH, between the hosts
  - A working KVM libvirt environment.
