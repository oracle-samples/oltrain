---
title: "Use Operators"
date: 2024-06-27
draft: false
summary: "Learn to deploy and use Operators with Oracle Cloud Native Environment."
tags: ["ocne", "lab", "tutorial", "ocne-install"]
showDate: true
---

## Links

:crescent_moon: [Lab](https://luna.oracle.com/lab/6f5e5b2e-f478-4a0f-8671-98d78a34aaf6)

:spiral_notepad: [Tutorial](https://docs.oracle.com/en/learn/ocne-operator)

## Details

A [Kubernetes operator](https://kubernetes.io/docs/concepts/extend-kubernetes/operator/) is a design pattern for writing code to automate tasks and extend Kubernetes. An operator is a set of concepts you can use to define a service for Kubernetes and helps to automate administrative services in Kubernetes.

The [Operator Lifecycle Manager module](https://docs.oracle.com/en/operating-systems/olcne/1.9/olm/) installs an instance of [Operator Lifecycle Manager](https://olm.operatorframework.io/) into a Kubernetes cluster to manage the installation and lifecycle of the operators. The Operator Lifecycle Manager references a public upstream operator registry ([https://operatorhub.io](https://operatorhub.io)) to share Operators. 

This tutorial shows how to install the Operator Lifecycle Manager module into your Oracle Cloud Native Environment cluster, followed by an example showing how to install and use an Operator.

### Objectives

In this tutorial, you will learn:

   - To install the `operator-lifecycle-manager` module
   - Verify the installation of the Operator Manager 
   - Install additional Operators

### Prerequisites

- Minimum of a 3-node Oracle Cloud Native Environment cluster:

   - Operator node
   - Kubernetes control plane node
   - Kubernetes worker node

- Each system should have Oracle Linux installed and configured with:

   - An Oracle user account (used during the installation) with sudo access
   - Key-based SSH, also known as password-less SSH, between the hosts
   - Installation of Oracle Cloud Native Environment with the OCI Cloud Controller Manager
