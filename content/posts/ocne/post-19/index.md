---
title: "Introducing Kubectl"
date: 2023-04-28
draft: false
summary: "Kubectl is a versatile tool used to deploy and inspect the configurations and logs of the cluster resources and applications."
tags: ["ocne", "lab", "tutorial", "ocne-k8s"]
showDate: true
---

## Links

:crescent_moon: [Introducing Kubectl with Oracle Cloud Native Environment](https://luna.oracle.com/lab/6c65a513-b161-47d2-b45c-92ca02e38dc0)

:spiral_notepad: [Introducing Kubectl with Oracle Cloud Native Environment](https://docs.oracle.com/en/learn/ocne-kubectl-intro)

## Details

Although graphical tools can manage Kubernetes, many administrators prefer to use command-line tools. The command line tool provided within the Kubernetes ecosystem is called [kubectl](https://kubernetes.io/docs/reference/kubectl/kubectl/). Kubectl is a versatile tool used to deploy and inspect the configurations and logs of the cluster resources and applications. Kubectl achieves this by using the Kubernetes API to authenticate with the Control Node of the Kubernetes cluster to complete any management actions requested by the administrator.

Most of the operations/commands available for kubectl provide administrators with the ability to deploy and manage applications deployed onto the Kubernetes cluster and inspect and manage the Kubernetes cluster resources. Because this lab is an introduction to kubectl, it will only focus on using kubectl to discover what Kubernetes resources are available in a new install of Oracle Cloud Native Environment.

> **Note:** Many kubectl commands have the `--all-namespaces` option appended. For this reason, a shorthand for this option is the `-A` flag. This lab uses kubectl `-A` instead of `kubectl --all-namespaces` in preference.

### Objectives

This tutorial introduces kubectl, a widely used command-line tool for interacting with a Kubernetes cluster. Beginning with why it is helpful to learn about it, the lab will also introduce some basic kubectl commands that help to understand any services deployed on a Kubernetes cluster, for example:

- location of the configuration file
- _kubectl config_
- _kubectl get_
- _kubectl describe_
- _kubectl version_

Most of these commands provide both _getter_ (to review settings) and _setter_ (to define/update settings) functions. This tutorial only uses kubectl to view the current configuration information.

### Prerequisites

- 5 Oracle Linux systems to use:
  - 1-off Operator node (ocne-operator)
  - 1-off Kubernetes control plane node (ocne-control)
  - 3-off Kubernetes worker node (ocne-worker)

Each system should have the latest Oracle Linux 8 (x86_64)

- The environment should be pre-configured with the following;
  - An oracle user account (used during the installation) with sudo access
  - Key-based SSH, also known as passwordless SSH, between the hosts
  - Installation of Oracle Cloud Native Environment and CCM module
