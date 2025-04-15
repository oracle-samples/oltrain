---
title: "Build From Source"
date: 2025-04-15
draft: false
summary: "Learn how to build Oracle Cloud Native Environment from the GitHub source code."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/cbb51122-f393-454e-96f2-0486402b1f1d)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-build)

## Details

The Oracle Cloud Native Environment (Oracle CNE) Command Line Interface (CLI) manages the lifecycle of the Kubernetes cluster at your organization. It is also an Open Source project available on [GitHub](https://github.com/oracle-cne/ocne), and this tutorial demonstrates how to build the `ocne` executable yourself. 

For more information about Oracle Cloud Native Environment 2, please refer to the current [Release Documentation](https://docs.oracle.com/en/operating-systems/olcne/) site.

### Objectives

In this tutorial, you'll learn to:

- Configure the build environment
- Build the `ocne` executable
- Start a Kubernetes cluster with the resulting executable

### Prerequisites

- Minimum of one Oracle Linux instance

- Each system should have Oracle Linux installed and configured with:

  - An Oracle user account (used during the installation) with sudo access
  - Key-based SSH, also known as password-less SSH, between the hosts
  - A working KVM libvirt environment.
