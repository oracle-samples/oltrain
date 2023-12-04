---
title: "Use Operator Lifecycle Manager to Deploy a Kubernetes Operator on Oracle Cloud Native Environment"
date: 2022-05-17
draft: false
summary: "This tutorial shows you how install the Operator Lifecycle Manager module for Oracle Cloud Native Environment into a Kubernetes cluster, then deploy a Kubernetes operator."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:spiral_notepad: [Use Operator Lifecycle Manager to Deploy a Kubernetes Operator on Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-olm)

## Details

This tutorial shows you how install the Operator Lifecycle Manager module for Oracle Cloud Native Environment into a Kubernetes cluster,
then deploy a Kubernetes operator. The Operator Lifecycle Manager module installs Operator Lifecycle Manager into a Kubernetes cluster. Operator Lifecycle Manager manages the installation and lifecycle management of Kubernetes operators in a Kubernetes cluster. This tutorial assumes you have an existing Kubernetes cluster running in Oracle Cloud Native Environment.

### Objectives

In this tutorial, you will learn how to:

- Install and configure the Operator Lifecycle Manager
- Use a Kubernetes Operator

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
