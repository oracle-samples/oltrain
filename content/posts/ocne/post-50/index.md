---
title: "Use ock-forge"
date: 2025-04-28
draft: false
summary: "Learn how to configure ock-forge to prepare image resources to use with an Oracle Cloud Native Environment cluster."
tags: ["ocne2", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/c77bc587-0d5e-45cf-9cc5-6d41daac0ec6)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne2-ock-forge)

## Details

The [Oracle Container Host for Kubernetes Image Builder (OCK Image Builder)](https://github.com/oracle-cne/ock-forge) tool builds the Oracle Container Host for Kubernetes (OCK) images used in Oracle Cloud Native Environment (Oracle CNE) deployments. OCK Image Builder helps if the default OCK image used by Oracle CNE does not meet your requirements like needing:

- A partition layout different from the standard OCK image.
- Extra packages or missing device drivers.

OCK Image Builder is a collection of shell scripts, the primary one being `ock-forge` to generate a bootable qcow2 format image to create the cluster nodes or an OSTree container image that Oracle CNE can use to update nodes in a running container.

### Objectives

In this tutorial, you will learn to:

- Install, set up, and use `ock-forge` to build a customized OCK image
- Create an Oracle CNE cluster using the customized OCK image
- Include `extraIgnitionInline:` changes to the OCK image either as a default for all clusters created or when used with an individual cluster

### Prerequisites

- Minimum of one Oracle Linux 9 instance

- Each system should have Oracle Linux installed and configured with:

  - An Oracle user account (used during the installation) with sudo access
  - Key-based SSH, also known as password-less SSH, between the hosts
  - A working KVM libvirt environment.
