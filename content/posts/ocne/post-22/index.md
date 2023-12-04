---
title: "Use ConfigMaps and Secrets"
date: 2023-09-29
draft: false
summary: "This tutorial shows how to create and use ConfigMaps and Secrets with Oracle Cloud Native Environment."
tags: ["ocne", "lab", "tutorial"]
showDate: true
---

## Links

:crescent_moon: [Use ConfigMaps and Secrets with Oracle Cloud Native Environment](https://luna.oracle.com/lab/14984256-1691-4d7a-8468-6ff38b6253ad)

:spiral_notepad: [Use ConfigMaps and Secrets with Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-configmap)

## Details

This tutorial shows how to create and use ConfigMaps and Secrets with Oracle Cloud Native Environment. Both ConfigMaps and Secrets are used to define configuration data and have many similarities. You will start by covering how to use ConfigMaps, and then cover the use of Secrets.

### Objectives

You will learn:

- Use ConfigMaps and Secrets with Oracle Cloud Native Environment.

### Prerequisites

- 3 Oracle Linux systems to use as:
  - Operator node (ocne-operator-01)
  - Kubernetes control plane node (ocne-control-01)
  - Kubernetes worker node (ocne-worker-01)

- Each system should have the latest Oracle Linux 8 (x86_64) installed

- This environment is pre-configured with:
  - An Oracle user account (used during the installation) with sudo access
  - Key-based SSH, also known as password-less SSH, between the hosts
  - Installation of Oracle Cloud Native Environment and Oracle Cloud Infrastructure Cloud Controller Manager (oci-ccm) module
